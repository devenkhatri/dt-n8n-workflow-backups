# Workflow Analysis for Add new clients from Notion to Clockify

## Description
This workflow automatically syncs new client entries from a Notion database to Clockify, ensuring your time tracking workspace stays up to date with your client list.

## Input Details
The workflow is triggered by new entries in a specified Notion database, polling for changes every minute.

## Process Summary
The workflow starts by polling a Notion database for new client records at a set interval (every minute). When a new client is detected, it extracts the client name from the Notion entry. It then uses this data to create a new client in a specified Clockify workspace. The workflow includes error handling to manage failures during execution. Sticky notes provide setup instructions for Notion and Clockify configurations.

## Output Details
The workflow creates a new client in Clockify using the name from the Notion database entry.

## Tags
automation, n8n, production-ready, excellent, optimized, Notion, Clockify, client sync
