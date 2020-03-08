---
id: read-pdf-file
title: Read PDF File (Deprecated)
---

`Deprecated`

Loads the contents and metadata of a PDF file into context.

## Script Data
---

| **Name** | **Description** |
| --- | --- |
| Script Type | python |
| Tags | Utility, ingestion |
| Demisto Version | 4.1.0 |

## Inputs
---

| **Argument Name** | **Description** |
| --- | --- |
| entryID | The War Room entryID of the file to read. |
| maxFileSize | The maximal file size to load, in bytes. The default is 1MB. |

## Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| URL.Data | The list of URLs that were extracted from the PDF file. | Unknown |
| File.Text | The PDF file's extracted text. | Unknown |
| File.Producer | The PDF file's producer. | Unknown |
| File.Title | The PDF file's title. | Unknown |
| File.xap | The PDF file's XAP. | Unknown |
| File.Author | The PDF file's author. | Unknown |
| File.dc | The PDF file's DC. | Unknown |
| File.xapmm | The PDF file's XAPMM. | Unknown |
| File.ModDate | The PDF file's modification date. | Unknown |
| File.CreationDate | The PDF file's creation date. | Unknown |
| File.Pages | The number of pages in the PDF file. | Unknown |
