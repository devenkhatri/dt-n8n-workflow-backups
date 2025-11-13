# Workflow Analysis for Googlesheetstrigger Workflow

## Description
This workflow automatically checks new email entries in a Google Sheet for duplicates, validates their deliverability using an external API, and updates the sheet with the validation status.

## Input Details
The workflow is triggered by new or updated rows in a specified Google Sheet, polling every minute for changes.

## Process Summary
The workflow starts by polling a Google Sheet for new data every minute. It removes duplicate entries based on the Email field. Each unique email is then sent to an external email validation API via an HTTP POST request. The response from the API is used to update the corresponding row in the original Google Sheet with the validation result. An 'If' condition checks whether a 'Status' field already exists before proceeding with updates.

## Output Details
The workflow updates the original Google Sheet with the email validation status returned by the external API.

## Tags
Google Sheets, email validation, automation, deduplication, API integration, data enrichment, n8n
