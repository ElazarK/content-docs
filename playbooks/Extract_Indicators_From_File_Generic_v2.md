---
id: extract-indicators-from-file-generic-v2
title: Extract Indicators From File Generic V2
---

Extracts indicators from a file.

Supported file types:
- PDF
- TXT
- HTM, HTML
- DOC, DOCX

## Dependencies
This playbook uses the following sub-playbooks, integrations, and scripts.

### Sub-playbooks
This playbook does not use any sub-playbooks.

### Integrations
This playbook does not use any integrations.

### Scripts
* Set
* ExtractIndicatorsFromTextFile
* ExtractIndicatorsFromWordFile
* ReadPDFFileV2

### Commands
* image-ocr-extract-text

## Playbook Inputs
---

| **Name** | **Description** | **Default Value** | **Source** | **Required** |
| --- | --- | --- | --- | --- |
| File | The file from which to extract indicators. | None | File | Optional |

## Playbook Outputs
---

| **Path** | **Description** | **Type** |
| --- | --- | --- |
| Domain.Name | The extracted domains. | unknown |
| Account.Email.Address | The extracted emails addresses. | unknown |
| File.MD5 | The extracted MD5 hash of the file. | unknown |
| File.SHA1 | The extracted SHA1 hash of the file. | unknown |
| File.SHA256 | The extracted SHA256 hash of the file. | unknown |
| IP.Address | The extracted IP addresses. | unknown |
| File.Text | The text or images extracted from the PDF file. | unknown |
| File.Producer | The producer of the PDF file. | unknown |
| File.Title | The title of the PDF file. | unknown |
| File.xap | The XAP of the PDF file. | unknown |
| File.Author | The author of the PDF file. | unknown |
| File.dc | The DC of the PDF file. | unknown |
| File.xapmm | The XAPMM of the PDF file. | unknown |
| File.ModDate | The modified date of the PDF file. | unknown |
| File.CreationDate | The creation date of the PDF file. | unknown |
| File.Pages | The number of pages in the PDF file. | unknown |
| URL.Data | The list of URLs that were extracted from the PDF file. | unknown |

![Extract_Indicators_From_File_Generic_v2](https://github.com/ElazarK/content-docs/blob/master/images/playbooks/Extract_Indicators_From_File_Generic_v2.png)
