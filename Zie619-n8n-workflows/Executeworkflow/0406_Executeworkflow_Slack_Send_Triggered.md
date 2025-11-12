# Workflow Analysis for AI Agent with Fallback to Human Support via Slack

## Description
This workflow implements an AI chat agent that responds to user messages. When the AI doesn't know the answer, it uses a custom tool to check if the user provided an email address. If an email is present, it sends a message to a Slack support channel and confirms to the user that a human will assist. If no email is provided, it asks the user to resend their question with an email address.

## Input Details
The workflow is triggered by an incoming chat message and may also be called as a sub-workflow with a 'chatInput' parameter containing the user's message.

## Process Summary
The main AI agent receives a chat message and, when uncertain, calls a sub-workflow. The sub-workflow checks if the user's message contains an email address using regex. If an email is found, it sends a help request to a Slack channel and returns a confirmation message to the user. If no email is found, it prompts the user to include an email in their query. The workflow uses memory to retain conversation context and integrates with OpenAI for chat responses.

## Output Details
The workflow either returns a prompt asking for an email or a confirmation that a human has been notified via Slack, depending on whether an email was provided in the user's message.

## Tags
AI agent, chatbot, Slack integration, email validation, fallback support, sub-workflow, OpenAI, customer support, workflow automation, n8n
