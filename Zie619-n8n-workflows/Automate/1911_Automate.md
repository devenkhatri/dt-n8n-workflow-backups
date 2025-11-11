# Workflow Analysis for lemlist <> GPT-3

## Description
This workflow automatically processes replies to sales emails by analyzing the content with AI to determine the appropriate action—such as unsubscribing the lead, creating a follow-up task, or logging a new deal in HubSpot—based on the reply's intent.

## Input Details
The workflow is triggered manually or by an incoming webhook when a lead replies to a lemlist email campaign, providing data like the reply text, lead email, campaign ID, and lead identifiers.

## Process Summary
The workflow starts by receiving a lead's email reply via webhook or manual trigger. It uses OpenAI's GPT-3 to categorize the reply into one of four categories: 'interested', 'Out of office', 'unsubscribe', or 'other'. Based on the AI's classification, the workflow routes execution through a switch node. If the reply indicates interest, it creates a new deal in HubSpot and adds a follow-up task. If the reply is an out-of-office message or unsubscribe request, it updates the lead's status in lemlist accordingly. Errors during execution are caught and handled by a dedicated error node.

## Output Details
The workflow updates external systems based on the email reply: it may create a HubSpot deal, add a follow-up task, or unsubscribe the contact in lemlist, and it can also send notifications or logs via webhook.

## Tags
AI, email automation, lead management, HubSpot, lemlist, OpenAI, sales workflow, categorization, unsubscribe handling, deal creation
