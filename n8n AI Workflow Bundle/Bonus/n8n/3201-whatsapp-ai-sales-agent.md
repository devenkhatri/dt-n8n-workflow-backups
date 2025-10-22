# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI, providing instant responses and managing sales inquiries efficiently.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow receives a WhatsApp message and extracts the contact number and message text. It then interacts with an AI model (OpenAI GPT-4) to generate a relevant response based on the conversation history and a predefined persona. The AI agent analyzes the message, retrieves lead information from a Google Sheet if the contact is new, and constructs a personalized reply. Finally, it formats the AI-generated response and sends it back to the customer on WhatsApp.

## Output Details
The workflow responds to the customer on WhatsApp with an AI-generated message.
