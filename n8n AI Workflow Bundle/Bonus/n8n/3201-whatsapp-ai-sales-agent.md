# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent, allowing businesses to respond to queries and provide information efficiently.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by extracting the incoming message and phone number. It then checks if the user has an existing chat history in a Google Sheet. If not, a new chat history is created. The workflow determines if the AI should respond or if the message should be escalated to a human, based on the AI’s confidence score. If the AI responds, it uses OpenAI to generate a relevant message, which is then sent back to the user on WhatsApp. The chat history is always updated in the Google Sheet.

## Output Details
The workflow sends automated AI-generated responses or escalation messages back to the customer on WhatsApp and maintains a chat history in a Google Sheet.
