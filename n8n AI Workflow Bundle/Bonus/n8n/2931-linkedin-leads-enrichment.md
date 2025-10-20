# Workflow Analysis for LinkedIn Lead Enrichment Workflow

## Description
This workflow automates the process of enriching LinkedIn lead data by extracting information from user-provided LinkedIn profile URLs, obtaining their email addresses, and then appending all this information to a Google Sheet.

## Input Details
The workflow is triggered manually and receives LinkedIn profile URLs as input.

## Process Summary
The workflow starts by extracting the full name and company name from the provided LinkedIn profile URL. It then uses Hunter.io to find the email address associated with the extracted full name and company. Finally, it formats the collected data (LinkedIn URL, full name, company, and email) and appends it as a new row to a specified Google Sheet.

## Output Details
The workflow outputs enriched lead data (LinkedIn URL, full name, company, and email) to a Google Sheet.
