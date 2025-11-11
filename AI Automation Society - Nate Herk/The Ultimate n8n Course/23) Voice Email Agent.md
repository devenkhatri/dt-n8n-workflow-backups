# Workflow Analysis for Voice Email Agent

## Description
This workflow receives email drafting requests via a webhook, uses an AI agent to look up the recipient's email address from a Google Sheet, generates a professional email using OpenAI, and sends it via Gmail.

## Input Details
The workflow is triggered by a POST webhook request containing the recipient's name and desired email content.

## Process Summary
The workflow starts when a webhook receives a request with the recipient's name and email content. An AI agent uses this information to first query a Google Sheet to find the recipient's email address. Using the retrieved email address and the provided content, the AI agent drafts a professional email with a subject and body. The agent then sends the email via Gmail. Finally, the workflow responds to the original webhook request to confirm completion.

## Output Details
The workflow sends a professionally drafted email to the recipient via Gmail and returns a response to the webhook that triggered the workflow.

## Tags
AI Agent, Email Automation, Webhook, Google Sheets, Gmail, OpenAI
