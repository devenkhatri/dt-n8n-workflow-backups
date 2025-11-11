# Workflow Analysis for Airtable PDF Data Extraction with Dynamic Prompts

## Description
This workflow automatically extracts data from PDFs uploaded to an Airtable table using AI-powered prompts defined in the table's field descriptions. When a row is updated or a field is created/modified, the workflow intelligently processes only the necessary data and updates the corresponding records.

## Input Details
The workflow is triggered by Airtable webhook events for 'row.updated', 'field.created', or 'field.updated' and receives event payload data including table schema, record IDs, and field information.

## Process Summary
The workflow first parses the incoming Airtable webhook event to determine the type of change (row or field). It fetches the table schema to identify fields with descriptions (prompts). For row updates, it processes only rows with PDF files and missing field values. For field changes, it updates all relevant rows. It downloads PDFs, extracts text, and uses an LLM with dynamic prompts to generate field values based on the PDF content and field descriptions. Finally, it updates the Airtable records with the extracted data.

## Output Details
The workflow updates Airtable records with AI-extracted data from PDFs, populating fields based on user-defined prompts in the field descriptions.

## Tags
Airtable, PDF extraction, LLM, dynamic prompts, webhook, automation, AI, data extraction, document processing, no-code
