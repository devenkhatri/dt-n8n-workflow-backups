# Workflow Analysis for Pipedrive Workflow

## Description
This workflow automatically processes email replies from cold email campaigns, determines if the recipient is interested in a meeting using AI, and creates a deal in Pipedrive CRM if they are qualified as interested.

## Input Details
The workflow is triggered by incoming emails from one or more Gmail inboxes, capturing the email content for processing.

## Process Summary
The workflow starts by monitoring Gmail inboxes for new replies. It extracts the email text and searches for the sender in Pipedrive CRM using their email address. If the person exists and is marked as part of a campaign, the workflow sends the email exchange to OpenAI’s GPT-4 to assess interest. The AI response is parsed to determine if the lead is interested, and if so, a new deal is created in Pipedrive linked to that person.

## Output Details
If a lead is deemed interested, a new deal is created in Pipedrive CRM; otherwise, no action is taken.

## Tags
CRM, Pipedrive, Gmail, OpenAI, email automation, lead qualification, sales automation, AI analysis
