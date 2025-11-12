# Workflow Analysis for ProspectLens company research

## Description
This workflow automates company research by pulling data from a Google Sheet, enriching it using the ProspectLens API, and updating the sheet with detailed company information such as funding, traffic, location, and founding year.

## Input Details
The workflow is manually triggered and reads rows from a predefined Google Sheet that contains company domains, processing only those with an empty 'processed_at' field.

## Process Summary
The workflow starts by manually triggering and fetching all rows from a Google Sheet. It filters rows where the 'processed_at' field is empty to identify unprocessed companies. Each unprocessed row is processed individually using a loop to maintain low concurrency. For each company, it calls the ProspectLens API to retrieve detailed company data. Finally, it updates the original Google Sheet row with enriched data including name, description, funding, traffic, location, and a timestamp in the 'processed_at' field.

## Output Details
The workflow updates the original Google Sheet with enriched company data and marks each processed row with a timestamp in the 'processed_at' column.

## Tags
automation,n8n,production-ready,excellent,optimized,google-sheets,prospectlens,company-research,api-integration
