# Workflow Analysis for Qualify New Leads in Google Sheets via OpenAI's GPT-4

## Description
This workflow automatically qualifies new leads entered into a Google Sheet using OpenAI's GPT-4 based on criteria such as decision-making authority, team size, and email domain. It ensures that only quality leads are identified for further action.

## Input Details
The workflow is triggered when a new row (representing a new lead) is added to a specified Google Sheet.

## Process Summary
1. The workflow is initiated when a new lead entry is detected in a Google Sheet. 2. It then sends the lead's information (name, email, business area, team size) to OpenAI's GPT-4 for qualification. 3. GPT-4 evaluates the lead based on criteria like the lead's role (decision-maker), team size, and email domain, returning a qualification rating and explanation in JSON format. 4. The JSON response from GPT-4 is extracted and parsed. 5. Finally, the original lead data is merged with the qualification results.

## Output Details
The workflow updates the original Google Sheet by adding a 'Rating' for each lead based on the qualification provided by GPT-4.

## Tags
automation, n8n, production-ready, excellent, optimized, Google Sheets, OpenAI, Lead Qualification, GPT-4
