# Workflow Analysis for Airtable Dynamic PDF Data Extraction with LLM

## Description
This workflow automatically extracts data from PDF files stored in an Airtable record and populates other fields in the same record based on user-defined prompts in the field descriptions. It reacts to Airtable events such as row updates or field changes, uses an AI language model to interpret the PDF content according to each field's prompt, and updates the Airtable record with the extracted values.

## Input Details
The workflow is triggered by Airtable webhook events (row.updated, field.created, or field.updated) and receives event payload data including base ID, table ID, row ID, and/or field ID.

## Process Summary
When triggered, the workflow first fetches the Airtable table schema to identify fields with user-defined prompts (descriptions). Depending on the event type, it either processes a single updated row or all rows affected by a field change. For each relevant row, it downloads the PDF from the designated 'File' field, extracts text, and uses an LLM to generate field values based on the prompts. Finally, it updates the Airtable record with the extracted data.

## Output Details
The workflow updates Airtable records with AI-extracted data from PDFs, populating fields according to user-defined prompts in the field descriptions.

## Tags
Airtable, PDF extraction, LLM, AI automation, dynamic prompts, webhook, data extraction, no-code AI, document processing, field automation
