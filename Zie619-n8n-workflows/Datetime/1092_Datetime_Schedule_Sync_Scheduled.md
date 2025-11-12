# Workflow Analysis for Two Way Sync Pipedrive and MySQL

## Description
This workflow keeps contact information synchronized between a MySQL database and Pipedrive CRM by periodically comparing records and updating whichever system has older data.

## Input Details
The workflow is triggered on a schedule and pulls contact data from both MySQL (via a SELECT query) and Pipedrive (via API).

## Process Summary
First, the workflow fetches all contacts from MySQL and Pipedrive. It then normalizes the Pipedrive data to match the MySQL schema. Using a dataset comparison node, it identifies matching records by email and detects differences in name, phone, or update timestamps. For differing records, it checks which side was updated more recently and propagates those changes to the other system—either updating the Pipedrive person or the MySQL contact record accordingly.

## Output Details
The workflow updates records in both Pipedrive and MySQL to ensure they remain in sync, with changes always flowing from the most recently updated source.

## Tags
two-way sync, Pipedrive, MySQL, CRM sync, contact synchronization, data consistency, automation, n8n, production-ready
