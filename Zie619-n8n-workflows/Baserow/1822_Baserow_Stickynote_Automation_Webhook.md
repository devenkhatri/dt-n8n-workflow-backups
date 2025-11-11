# Workflow Analysis for Baserow markdown to html

## Description
This workflow automatically converts markdown-formatted video descriptions stored in a Baserow database into HTML. It can process either a single record or all records in a table, depending on the trigger input.

## Input Details
The workflow is triggered via a webhook that may include a query parameter specifying a single record ID to process; if no record ID is provided, it processes all records.

## Process Summary
The workflow starts with a webhook trigger and checks if a specific record ID is provided. If a record ID is present, it fetches that single record from Baserow; otherwise, it retrieves all records from the specified table. It then converts the '📥 Video Description' field from markdown to HTML using a markdown conversion node. Finally, it updates the corresponding record(s) in Baserow with the generated HTML in a designated field.

## Output Details
The workflow updates the Baserow records with the converted HTML version of the markdown video description in a specified field.

## Tags
automation, n8n, production-ready, excellent, optimized, baserow, markdown, html, webhook
