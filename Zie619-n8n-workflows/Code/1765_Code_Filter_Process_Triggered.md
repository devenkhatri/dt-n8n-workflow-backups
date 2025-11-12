# Workflow Analysis for Colombian Invoices Processing

## Description
This workflow automatically processes electronic invoices received via Gmail in Colombia by extracting key details from attached ZIP files containing PDF and XML documents, validating the data, and storing it in Google Drive and Google Sheets.

## Input Details
The workflow is triggered every 30 minutes by new Gmail messages containing ZIP file attachments, which are assumed to include Colombian electronic invoices in PDF and XML formats.

## Process Summary
The workflow starts by polling Gmail for emails with ZIP attachments. It extracts and filters only ZIP files, then unzips them to retrieve PDF and XML documents. Data is extracted from both file types, merged, and passed to an AI-powered parser (using OpenAI's GPT-4o-mini) that interprets and structures invoice details like invoice number, tax info, and CUFE. The workflow validates that the total equals subtotal plus tax using a calculator tool, then uploads the PDF to Google Drive with a standardized name and updates a Google Sheet with the parsed invoice data, using a unique key to avoid duplicates.

## Output Details
The workflow saves the original PDF to Google Drive with a formatted filename and logs structured invoice data into a Google Sheet, ensuring no duplicate entries.

## Tags
Colombia, invoice processing, Gmail, Google Drive, Google Sheets, PDF, XML, DIAN, OpenAI, automation, n8n, production-ready
