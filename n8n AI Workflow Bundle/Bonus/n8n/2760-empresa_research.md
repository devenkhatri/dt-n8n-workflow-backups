# Workflow Analysis for Company Research and Data Enrichment

## Description
This workflow automates the process of researching a given company, enriching its data using various APIs, generating a summary with AI, and then storing the results in a Google Sheet and sending an email notification.

## Input Details
The workflow is triggered manually and receives company names as input.

## Process Summary
The workflow starts by taking a company name and searching for its website using Google Search. It then extracts information about the business from its website using a custom tool. Next, it uses a company enrichment API to gather additional details and also enriches the data with Apollo.io. Finally, it uses an AI model to generate a descriptive summary of the company based on the collected information.

## Output Details
The enriched company data and AI-generated summary are appended to a specified Google Sheet, and an email notification is sent with the research results.
