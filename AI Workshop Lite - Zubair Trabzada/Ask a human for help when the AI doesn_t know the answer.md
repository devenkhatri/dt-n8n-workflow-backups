# Workflow Analysis for Ask a human

## Description
This workflow uses an AI agent to respond to user questions. If the AI doesn't know the answer or isn't confident, it triggers a sub-workflow that checks whether the user provided an email address. If an email is present, it sends a message to a Slack support channel; otherwise, it prompts the user to include their email for assistance.

## Input Details
The workflow is triggered by a chat message sent via a chat interface, containing the user's question in the 'chatInput' field.

## Process Summary
The AI agent attempts to answer the user's question using GPT-4. If unsure, it calls a custom tool that executes a sub-workflow. This sub-workflow checks if the user's message includes an email address using a regex condition. If an email is found, it sends the user's message to a Slack channel and confirms help is on the way. If no email is found, it replies asking the user to resend their question with an email address.

## Output Details
The workflow returns a chat response to the user—either an AI-generated answer, a request for an email, or a confirmation that a human has been notified via Slack.

## Tags
AI agent, human escalation, Slack integration, email validation, GPT-4, customer support, chatbot
