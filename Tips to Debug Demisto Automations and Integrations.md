# Tips to Debug Demisto Automations and Integrations

Use this article for the best practices to debug Demisto scripts and automations.

**Script** - for the purpose of this article **script** refers to either a Demisto automation or an integration as there is little difference troubleshooting either of them.

- [Output Debug Data](#Output-Debug-Data)
- [Debug Data with PPrint](#debug-data-with-pprint)
- [Unhandled Exceptions](#unhandled-exceptions)
- [How Did I Get Here? Stack Traces to the Rescue!](#how-did-i-get-here?-stack-traces-to-the-rescue!)

## Output Debug Data

A common method used to debug standard Python script is to put `print()` statements
throughout. For example, `print()` can be used to  troubleshoot flow control, see what data variables contain, and more. 

Demisto doesn’t provide TTY for scripts to output to, therefore using Python’s `print()` function, within Demisto, will not produce a viewable output. Demisto debugs using the command `demisto.log(“some text or variable”)`.

The `demisto.log()` command sends arbitrary text to the War Room. This command can be used without limit within a script. It differs from the `demisto.results()` command, which is typically run just once before a script completes.

When writing or troubleshooting scripts, it is recommended to use `demisto.log()` statements as needed in order to troubleshoot flow control and variable contents. Every use of the command will result in separate War Room entries for each `demisto.log()` statement.

**Example**:

```
my_var ='Lorem ipsum dolor sit amet, consectetur adipiscing elit'

demisto.log(my_var)
```

## Debug Data with PPrint

Complex data structures need to be read and debugged frequently. The `pprint` (“pretty print”) library which is built into Python can be used to help. Normally the `pprint.pprint()` command is used in development environments. However, since Demisto does not have a TTY, that command can not be used. Instead use the `pprint.pformat()` command. This command is different in that it returns a formatted string rather than outputting to the TTY.

`pformat()` will dump strings, lists, dictionaries, and tuples, and will format them in a way that makes sense, so that the internal structure can be seen. It will also identify the type of each part of the structure (whether it is a Python string, dict, or list). This provides invaluable information when debugging Demisto scripts.

**Example**: Given the following script with the name `DemistoPformatExample`:

```
from pprint import pformat
my_dict = {
  'keyboard': 'qwerty',
  'pi':3.14159265359,
  'car'':{
    'make': 'Aston Martin',
    'model': 'DB11',
    'year': 2019,
    'fuel': 'petrol'
  }
}
my_dicty['plane']={
 'make':'Cessna',
 'model':'172',
 'year':1981,
 'fuel':'100LL'
}

my_list=['a','b']
my_list.append('c')

  demisto.log( pformat( my_dict ) )

  demisto.log( pformat( my_list ) )
  ```

  ### War room output:

  ![Image](https://github.com/ElazarK/content-docs/blob/master/images/WarRoomOutput.png)

  ## Unhandled Exceptions

  Any unhandled exceptions in a script, which show errors in the War Room, but without useable context or line numbers, will not be helped with the `demisto.log()` statements. These statements will not produce any War Room output, even if they are placed in the code prior to where the exception will occur. You can troubleshoot this issue when it happens by using the `sys.exit()` command to terminate the script before the error occurs. If the exception still occurs, the `sys.exit()` command needs to be moved backwards in the code, line by line, until the script finishes with no exceptions being thrown. When an error is thrown, you will know that the next statement in the script is where the exception is. You can then concentrate on finding out why that statement threw the exception and fix it.

  **Example**:
  ```
   import sys

  def someFunc():
   good_code()
   demisto.log(‘some debug output’)
   sys.exit()#inserting sys.exit() can help isolate where the crash is occurring. The script won't
  complete, but if it doesn't crash either, you've got a pretty good idea where to look
   bad_line_of_code_that_is_crashing_python() # my code is failing here
   ```

## How Did I Get Here? Stack Traces to the Rescue!

When troubleshooting code written by someone else, if you know where the problem is, but you do not know how the code managed to enter the block, you may want to intentionally log a stack trace. The stack trace should take much of the guess work out of isolating the program flow.

The traceback Python library can help us out here. 

**Example**:

Given a simple automation called ‘**testStackTrace**’, we have three simple functions, a(), b(), and c(). We invoke c(), then c() invokes b(), and finally b() invokes a(), which then outputs a stack trace.

```
import traceback 
  def a():
   demisto.log(".join(traceback.format_stack())) # format_stack() returns a list, which we merge here
  
  def b():
   a()
  def c()
   b()
  
 c()
 ```

![Image](https://github.com/ElazarK/content-docs/blob/master/images/howdidigethere.png) 

The above screenshot shows the order in which the functions were called: c() ran first, which called b() second, which then called a() last. This shows exactly how our program arrived at function a()! 

This is a very simplistic example, but it can be an extremely powerful method of troubleshooting the program flow, if it would otherwise  be too tedious to troubleshoot.

**Top Tip**: The above screenshot has nothing to do with a thrown exception, it’s just output logged from a script.
