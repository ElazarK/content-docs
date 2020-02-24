Following a failed login attempt which happened more than 3 times, The user on Slack will be asked if they attempted a login. If not, the incident will be raided to a high level. If yes, the user will be asked if they need to reset their password and will reset the password in AD.

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
* slack

### Scripts
* ADExpirePassword
* CloseInvestigation
* SlackAskUser
* IncidentSet

### Commands
* slack-send

## Playbook Inputs
---
There are no inputs for this playbook.

## Playbook Outputs
---
There are no outputs for this playbook. 

![Failed_Login_With_Slack_Playbook](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Failed_Login_Playbook_With_Slack.png)
