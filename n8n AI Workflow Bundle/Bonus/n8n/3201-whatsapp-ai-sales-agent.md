# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It processes incoming messages, generates AI responses, and stores conversation data.

## Input Details
The workflow is triggered by incoming WhatsApp messages via a webhook.

## Process Summary
The workflow starts by retrieving the incoming WhatsApp message. It then checks the chat history for the contact. If it's a new conversation, it initializes a new chat session with an AI sales agent using OpenAI. For ongoing conversations, it appends the new message to the existing chat history and generates an AI response. Finally, it stores the conversation and sends the AI-generated message back to the customer on WhatsApp.

## Output Details
The workflow outputs AI-generated responses directly back to the customer via WhatsApp and stores conversation logs into a database.
