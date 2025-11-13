# Workflow Analysis for Airtable markdown to html

## Description
Automated workflow: Airtable markdown to html. This workflow integrates 6 different services: webhook, stickyNote, markdown, airtable, stopAndError. It contains 11 nodes and follows best practices for error handling and security.

## Input Details
This workflow is triggered by a webhook that receives data, specifically checking for a recordId in its query parameters to determine whether to process a single record or all records.

## Process Summary
The workflow is initiated by a webhook. It checks if a specific record ID is provided in the webhook query; if so, it fetches that single record from the "📺 Videos" Airtable table. Otherwise, it retrieves all records from the "📺 Videos" table, limited to 3 records. For each retrieved record, it converts the "📥 Video Description" field from markdown to HTML. Finally, it updates the respective record(s) in the Airtable "📺 Videos" table with the generated HTML content, also setting the "Unpublished" field to false if processing all records.

## Output Details
The workflow updates existing records in the "📺 Videos" table within the "360Creators" Airtable base by populating the "Video description HTML" field with the converted HTML content.

## Tags
automation,n8n,production-ready,excellent,optimized
