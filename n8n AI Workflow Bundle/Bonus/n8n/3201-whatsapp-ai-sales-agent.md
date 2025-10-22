# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It creates a conversational flow for sales inquiries, handles product questions, and saves lead information.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by extracting the customer's message and contact details from the incoming WhatsApp message. It then initializes a conversation with a pre-defined AI sales agent personality using OpenAI's API, providing the conversation history and a prompt. The AI generates a tailored response based on the customer's query. Finally, the AI's response is sent back to the customer via WhatsApp, and the customer's contact information is saved.

## Output Details
The workflow sends AI-generated sales responses back to the customer on WhatsApp and saves customer contact information.
