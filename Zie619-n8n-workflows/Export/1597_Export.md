# Workflow Analysis for Invoice Processing and Line Item Extraction Workflow

## Description
This workflow automatically processes invoice files uploaded to a Google Drive folder, extracts key line item details using AI, and saves the structured data into a database with proper linkage between invoices and their items.

## Input Details
The workflow is triggered when a new file is added to a specified Google Drive folder, and it receives the uploaded invoice file for processing.

## Process Summary
The workflow starts by detecting new invoice files in a Google Drive folder. It sends the file to LlamaParse for document parsing, and the parsed result is received via a webhook. Using OpenAI with a JSON schema, it extracts structured line item data (description, quantity, unit price, and amount) from the parsed content. The main invoice record is created in Airtable, and each line item is processed and stored as a linked record under the corresponding invoice.

## Output Details
The workflow creates a new invoice record in Airtable along with associated line item records, each containing parsed and validated details from the original invoice file.

## Tags
invoice processing, Google Drive, OCR, OpenAI, Airtable, line items, automation, document parsing, JSON schema, webhook
