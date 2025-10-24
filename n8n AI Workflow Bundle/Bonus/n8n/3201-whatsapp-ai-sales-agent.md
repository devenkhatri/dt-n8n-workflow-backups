# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interaction on WhatsApp using AI to answer queries and guide sales.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, it checks if the incoming message contains media. Then, it retrieves the conversation history from a Google Sheet and constructs a prompt for the Large Language Model (LLM). The LLM processes the message and generates a response, ensuring it adheres to a persona and provides relevant answers. This response is then formatted and sent back to the customer via WhatsApp. Finally, the conversation, including the new message and AI response, is appended to the Google Sheet.

## Output Details
The workflow sends an AI-generated response back to the customer on WhatsApp and updates a Google Sheet with the conversation history.
