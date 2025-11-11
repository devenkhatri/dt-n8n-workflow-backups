# Workflow Analysis for Email Search with Icypeas (Bulk Search)

## Description
This workflow automates bulk email searches using the Icypeas service by reading contact data from a Google Sheet, authenticating securely via API credentials, and submitting the data for email enrichment. Results are delivered via email and available for download in the Icypeas dashboard.

## Input Details
The workflow is manually triggered and reads contact data (firstname, lastname, company) from a specified Google Sheet.

## Process Summary
The workflow starts with a manual trigger, then reads contact data from a Google Sheet. It uses a code node to authenticate with Icypeas by generating a cryptographic signature using the user’s API key, secret, and user ID. The authenticated request, along with the contact data, is sent via an HTTP POST request to Icypeas’s bulk search endpoint. The Icypeas service processes the request asynchronously and delivers results via email and in the user's dashboard.

## Output Details
The workflow sends a bulk email search request to Icypeas; the actual email results are delivered via email from no-reply@icypeas.com and are available for download in the Icypeas web application.

## Tags
email search, bulk enrichment, Icypeas, Google Sheets, API authentication, manual trigger, n8n workflow
