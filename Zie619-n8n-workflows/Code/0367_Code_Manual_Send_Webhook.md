# Workflow Analysis for Batch Email Verification with Icypeas

## Description
This workflow automates bulk email verification by reading email addresses from a Google Sheet, authenticating with the Icypeas API using secure credentials, and submitting the emails for verification via a POST request.

## Input Details
The workflow is manually triggered and reads email data from a specified Google Sheet where the first column contains email addresses.

## Process Summary
The workflow starts with a manual trigger and reads email data from a Google Sheet. It then processes this data in a code node that formats the payload and generates a secure HMAC-SHA1 signature using the user's Icypeas API key and secret. The authenticated request, including the timestamp and signature in the headers, is sent to the Icypeas bulk email verification endpoint. The Icypeas service handles the verification asynchronously, and results are made available for download in the Icypeas dashboard and delivered via email.

## Output Details
The workflow sends a POST request to Icypeas to initiate bulk email verification; results are later accessed via the Icypeas web dashboard and delivered by email from no-reply@icypeas.com.

## Tags
email verification, Icypeas, bulk processing, Google Sheets, API authentication, HMAC signature, manual trigger, n8n workflow
