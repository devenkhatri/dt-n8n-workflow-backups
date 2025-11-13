# Workflow Analysis for Airtable Bulk CSV Upload Workflow

## Description
This workflow automates the process of uploading contact data from a CSV file into an Airtable base. When a new file is added via an Airtable form, the workflow downloads the file, reads its contents, and creates new lead records in a designated Airtable table while updating the upload status throughout the process.

## Input Details
The workflow is triggered when a new record is added to a specific Airtable 'Upload' table (via Airtable form), which includes a file attachment.

## Process Summary
The workflow starts by detecting a new upload in Airtable, then fetches the file ID and sets the status to 'Processing'. It downloads the attached CSV file and parses its contents. Before creating records, it checks if a 'Campaign' field is present and formats it accordingly. It then sends batched HTTP requests to Airtable to create lead records from the CSV rows. If successful, it updates the status to 'Uploaded'; if any error occurs, it marks the status as 'Failed'.

## Output Details
The workflow creates new lead records in an Airtable 'Leads' table and updates the status of the original upload record to 'Uploaded' or 'Failed'.

## Tags
Airtable, CSV upload, bulk import, automation, lead management, file processing, n8n, production-ready
