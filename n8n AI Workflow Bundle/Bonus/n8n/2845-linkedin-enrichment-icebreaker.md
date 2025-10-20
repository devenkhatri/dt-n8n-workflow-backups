# Workflow Analysis for LinkedIn Icebreaker Enrichment

## Description
This workflow enriches contact data using LinkedIn profiles and generates personalized icebreakers.

## Input Details
The workflow is manually triggered and receives contact data from a Google Sheet.

## Process Summary
The workflow starts by retrieving contact data from a specified Google Sheet. It then iterates through each contact, attempting to find their LinkedIn profile using their name and company. If a LinkedIn profile is found, the workflow extracts relevant information like job title, company, and recent activity. Finally, it uses an AI model to generate personalized icebreakers based on the extracted LinkedIn data.

## Output Details
The enriched contact data with generated icebreakers is updated back into the Google Sheet.
