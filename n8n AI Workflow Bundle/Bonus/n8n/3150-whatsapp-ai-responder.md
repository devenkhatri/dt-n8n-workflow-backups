# Workflow Analysis for WhatsApp AI Responder

## Description
This workflow automates responses to WhatsApp messages using AI, allowing for dynamic and intelligent conversations with users.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, the workflow extracts the incoming message and other relevant details from the webhook payload. Then, it constructs a prompt for the AI model based on the user's message and any previous conversation history. Next, it sends this prompt to a large language model (LLM) to generate a relevant response. Finally, the AI-generated response is sent back to the user via WhatsApp.

## Output Details
The workflow sends an AI-generated text response back to the user on WhatsApp.
