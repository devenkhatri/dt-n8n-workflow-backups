# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent to answer questions, recommend products, and assist with purchases.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, common data is set globally. Then, the workflow checks if the conversation is ongoing or if the user wants to end it. If the conversation continues, a prompt is prepared based on the chat history and product catalog, then sent to the AI agent. The AI agent's response is then prepared for WhatsApp and sent back to the user. Finally, the chat history in the Google Sheet is updated.

## Output Details
The workflow responds to the user's WhatsApp messages, providing AI-generated sales assistance and updating chat history in a Google Sheet.
