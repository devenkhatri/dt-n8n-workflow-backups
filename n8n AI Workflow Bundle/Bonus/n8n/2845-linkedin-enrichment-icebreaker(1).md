# Workflow Analysis for LinkedIn Enrichment Icebreaker

## Description
This workflow automates the process of enriching LinkedIn profiles and generating personalized icebreakers using AI, triggered by new or updated rows in a Google Sheet.

## Input Details
The workflow is triggered manually and processes data from a Google Sheet, using the "companyName" and "linkedinProfile" columns.

## Process Summary
The workflow starts by reading data from a Google Sheet, specifically company names and LinkedIn profile URLs. It then extracts the LinkedIn profile ID from each URL and uses this to fetch publicly available data from their LinkedIn pages. Following this, the workflow extracts the company name and generates a personalized icebreaker message using the OpenAI API. Finally, it formats the collected data to update the Google Sheet with the generated icebreaker message and other relevant information.

## Output Details
The workflow updates the Google Sheet with the extracted LinkedIn profile data, generated icebreaker message, and other relevant information.
