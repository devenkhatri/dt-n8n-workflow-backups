# Workflow Analysis for Invoice Processing Agent

## Description
This workflow automates the processing of incoming invoices by extracting data, generating a structured JSON, and sending it to a specified email address.

## Input Details
This workflow is triggered manually and receives invoice data from a Google Drive file.

## Process Summary
The workflow starts by reading a specified Google Drive file as binary data. This binary data is then converted into a base64 encoded string. The base64 encoded string, representing the invoice, is sent to a custom API for AI-powered data extraction. The extracted data from the invoice is then joined with predefined invoice details and converted into a JSON string.

## Output Details
The workflow sends the processed invoice data as a JSON string via email to a specified recipient.
