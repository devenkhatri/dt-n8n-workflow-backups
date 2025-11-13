# Workflow Analysis for TEMPLATES

## Description
Automated workflow: TEMPLATES. This workflow processes data and performs automated tasks.

## Input Details
This workflow is manually triggered and retrieves a specific item from Monday.com.

## Process Summary
1. The workflow starts with a manual trigger.
2. It fetches a specific item from Monday.com using a hardcoded item ID.
3. It then extracts the "Subitems" column value, parses it to get linked subitem IDs, and retrieves details for each subitem from Monday.com.
4. Concurrently, it extracts the "Additional Contacts" column value, parses it to obtain linked pulse IDs, and fetches details for each of these linked pulses from Monday.com.
5. There are also utility nodes for extracting specific column values by name or ID, converting data to a file, merging data, and a disabled node for uploading files to Monday.com.

## Output Details
The workflow retrieves and processes various linked item and column details from Monday.com.

## Tags
automation, n8n, production-ready, excellent, optimized
