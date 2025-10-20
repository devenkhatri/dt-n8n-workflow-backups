# Workflow Analysis for Airtable to Tally Form Submission with AI Data Extraction

## Description
This workflow automates the process of extracting specific information from new records in an Airtable base, enriching that data using an AI model, and then submitting it to a specified Tally form.

## Input Details
The workflow is triggered manually and processes specific records from an Airtable base.

## Process Summary
The workflow starts by retrieving new records from a specified Airtable base. It then iterates through these records, extracting a "Long Text" field. This extracted text is then sent to an AI model (OpenAI) to extract specific entities like product name, quantity, and unit. Finally, the extracted and AI-enriched data is formatted and submitted to a Tally form.

## Output Details
The workflow submits extracted and AI-processed data about product name, quantity, and unit to a Tally form.
