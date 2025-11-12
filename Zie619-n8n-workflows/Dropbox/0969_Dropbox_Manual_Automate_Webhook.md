# Workflow Analysis for Workflow management

## Description
This workflow automatically retrieves details of all n8n workflows, stores their metadata and JSON backup in Dropbox, and syncs key information like name, ID, CRON schedule, and trigger types to an Airtable database for centralized monitoring and management.

## Input Details
The workflow is triggered either manually via the 'On clicking execute' node or automatically via a CRON schedule every hour at 15 and 45 minutes past the hour.

## Process Summary
The workflow first fetches a list of all workflows via an HTTP request. It then processes each workflow individually: retrieving its full details, saving its JSON definition to Dropbox, and generating a shareable file link. It analyzes the workflow’s nodes to detect if it uses CRON or trigger nodes. It then checks if a record for the workflow already exists in Airtable; if so, it updates the record, otherwise it creates a new one with key metadata and file link.

## Output Details
The workflow outputs updated or newly created records in an Airtable 'Workflows' table and stores workflow JSON backups in Dropbox with versioned filenames based on workflow ID and last update time.

## Tags
workflow management, n8n, Airtable, Dropbox, CRON detection, backup automation, metadata sync, production-ready
