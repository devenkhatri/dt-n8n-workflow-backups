# Workflow Analysis for Typeform Lead Workflow

## Description
This workflow automates lead management by capturing Typeform submissions, updating or creating contacts in HubSpot, enriching company data with Clearbit, and notifying via email and Slack.

## Input Details
The workflow is triggered by new Typeform submissions.

## Process Summary
First, the workflow receives submission data from Typeform. Then, it checks if a contact with the submitted email already exists in HubSpot. If not, it creates a new contact in HubSpot. Concurrently, it uses Clearbit to find company information based on the submitted email. Finally, all the collected information is compiled and sent as notifications via email and Slack.

## Output Details
The workflow updates or creates contacts in HubSpot, enriches data, and sends notifications via email and Slack.
