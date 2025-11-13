# Workflow Analysis for Qualify new leads in Google Sheets via OpenAI's GPT-4

## Description
This workflow automates the process of qualifying new leads submitted through a Google Sheet by leveraging OpenAI's GPT-4 for lead assessment. It is designed for production use, incorporating error handling and security best practices.

## Input Details
The workflow is triggered automatically whenever a new entry (lead) is added to a specified Google Sheet, receiving the lead's information.

## Process Summary
The workflow starts by monitoring a Google Sheet for new lead entries. Once a new lead is detected, its details (name, email, business area, team size) are sent to OpenAI's GPT-4. GPT-4 qualifies the lead based on predefined criteria, specifically looking for decision-makers and corporate email domains, and returns a rating and an explanation in JSON format. The JSON response from GPT-4 is parsed to extract the lead qualification rating. The original lead data from the Google Sheet is then merged with the extracted qualification rating. Finally, the workflow updates the Google Sheet by adding the new qualification rating to the corresponding lead entry.

## Output Details
The workflow updates the Google Sheet where the leads originate by adding a 'Rating' to each processed lead entry.

## Tags
automation, n8n, Google Sheets, OpenAI, GPT-4, Lead Qualification, AI, data processing, sales, marketing
