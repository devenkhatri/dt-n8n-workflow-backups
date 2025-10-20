# Workflow Analysis for AI WhatsApp Support Bot

## Description
This workflow automates customer support on WhatsApp using AI. It receives messages from WhatsApp, processes them using a custom AI model, stores the conversation, and sends automated replies.

## Input Details
The workflow is triggered by incoming messages to a WhatsApp Business Account via a webhook.

## Process Summary
The workflow starts by receiving a WhatsApp message. It then retrieves the customer's conversation history from Google Sheets. This history, along with the new message, is sent to a custom AI model (via OpenAI's GPT-3.5-turbo) to generate a relevant response. The new message and the AI-generated response are appended to the conversation history in Google Sheets. Finally, the AI-generated response is sent back to the customer via WhatsApp.

## Output Details
The workflow sends automated, AI-generated replies directly to the customer's WhatsApp.
