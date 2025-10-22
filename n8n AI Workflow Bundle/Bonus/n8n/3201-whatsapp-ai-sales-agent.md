# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent, allowing businesses to respond to queries and provide information efficiently.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, the workflow extracts the sender's phone number and the incoming message from the webhook data. Then, it initializes a conversation with an AI agent using OpenAI to process the message and generate a suitable response. Next, it formats the AI-generated response into a structured message adaptable for WhatsApp. After that it sends the formatted AI message back to the customer via WhatsApp. Finally, it dynamically manages conversation history and context to ensure relevant and continuous AI interaction.

## Output Details
The workflow sends automated, AI-generated responses back to the customer's WhatsApp.
