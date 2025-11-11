# Workflow Analysis for Googledrive Workflow

## Description
This workflow automatically processes new invoices added to a specific Google Drive folder by extracting line item details using AI and saving the structured data into an Airtable database.

## Input Details
The workflow is triggered when a new file is added to a designated Google Drive folder containing invoices.

## Process Summary
First, the Google Drive trigger detects a newly uploaded invoice file. The file is then downloaded and sent via an HTTP request to an external parsing service (LlamaParse) with instructions to extract invoice line items. The parsed data is received through a webhook and processed using OpenAI's GPT model to ensure it conforms to a predefined JSON schema. The validated line items are then split into individual records and stored in Airtable, with one record created for the invoice and separate linked records for each line item.

## Output Details
The workflow creates structured invoice and line item records in an Airtable base for tracking and analysis.

## Tags
invoice processing, Google Drive, Airtable, AI extraction, document parsing, automation, webhook, OpenAI, LlamaParse, n8n
