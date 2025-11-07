# Workflow Analysis for AI-Powered Sales Lead Email Automation from Airtable

## Description
This workflow automates personalized email communication for sales leads by monitoring their status in Airtable, selecting appropriate email templates from Google Docs, and utilizing an AI agent to customize and draft emails before sending them via Gmail.

## Input Details
The workflow is triggered every minute by an Airtable record in the "Leads/clients" base when the "Status" field changes, receiving lead details such as name and email address.

## Process Summary
1. The workflow starts by polling an Airtable base for updates to lead records, specifically changes in their 'Status' field.
2. Depending on the detected lead status, the workflow intelligently selects a corresponding email template from one of six Google Docs.
3. An AI agent, powered by an OpenAI chat model, then receives the lead's name and the selected email template.
4. The AI agent's role is to personalize the email template by dynamically inserting the lead's name into both the email body and the subject line, ensuring professional formatting.
5. Finally, the personalized email is drafted and sent to the lead's email address using the Gmail tool.

## Output Details
The workflow produces and sends a dynamically generated, personalized email to the respective sales lead's email address through Gmail.
