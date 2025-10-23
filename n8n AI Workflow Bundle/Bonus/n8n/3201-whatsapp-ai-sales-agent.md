# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It processes incoming messages, generates AI responses, and stores conversation history in Google Sheets.

## Input Details
The workflow is triggered by incoming messages to a WhatsApp Business Account webhook.

## Process Summary
The workflow receives a new WhatsApp message, extracts sender and message details, and retrieves previous conversation history from Google Sheets. It then uses OpenAI to generate an appropriate response based on the conversation history and a predefined sales persona. Finally, the generated AI response is sent back to the customer via WhatsApp and the entire conversation is updated in the Google Sheet.

## Output Details
The workflow sends AI-generated sales responses back to the customer on WhatsApp and archives the conversation history in a Google Sheet.
