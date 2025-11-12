# Workflow Analysis for Googlesheetstrigger Workflow

## Description
This workflow monitors a Google Sheet for changes in the 'Security Code' column and automatically sends an ASCII-formatted table of selected investment data (Security Code, Price, Quantity) to a Discord channel whenever a row is added or updated.

## Input Details
The workflow is triggered when a new row is added or an existing row is updated in a specified Google Sheet, specifically watching changes in the 'Security Code' column.

## Process Summary
The workflow starts by polling a Google Sheet every minute to detect changes in the 'Security Code' column. When a change is detected, it retrieves all rows from the sheet. A code node then formats the data for specific columns ('Security Code', 'Price', 'Quantity') into an ASCII table. This formatted table is then sent as a message to a Discord channel via a webhook. Error handling is included to manage any failures during execution.

## Output Details
The workflow outputs a formatted ASCII table message to a Discord channel via a webhook URL whenever sheet data changes.

## Tags
Google Sheets, Discord, automation, table formatting, webhook, monitoring, n8n
