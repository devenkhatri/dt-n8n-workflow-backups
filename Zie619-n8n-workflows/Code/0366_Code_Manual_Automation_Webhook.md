# Workflow Analysis for Domain Scan with Icypeas (Bulk Search)

## Description
This workflow automates bulk domain scanning by reading company names from a Google Sheet, authenticating with the Icypeas API using cryptographic signatures, and submitting the data for processing. Results are delivered via email and available in the Icypeas web application.

## Input Details
The workflow is manually triggered and reads company names from a specified Google Sheet where the first column is labeled 'company'.

## Process Summary
The workflow starts with a manual trigger, then reads company names from a connected Google Sheet. It prepares authentication data—including an API key, secret, user ID, and a cryptographic signature—for the Icypeas bulk search API. Using this data, it sends a POST request to the Icypeas API to initiate a domain scan task. After submission, the results are processed asynchronously by Icypeas and delivered via email and the Icypeas dashboard.

## Output Details
The workflow sends a bulk domain scan request to Icypeas and does not directly return results; users receive scan results via email and can download them from the Icypeas web application.

## Tags
domain scan, Icypeas, bulk search, Google Sheets, API authentication, crypto signature, manual trigger, n8n workflow
