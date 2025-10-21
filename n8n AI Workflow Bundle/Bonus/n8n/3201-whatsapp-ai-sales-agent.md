# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent, allowing businesses to respond to queries and provide information efficiently.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, the workflow receives a new WhatsApp message. It then processes the message content and uses an AI model (OpenAI GPT-4) to generate a relevant response based on a predefined prompt, product knowledge, and chat history. After getting the AI-generated response, it translates the message into a format suitable for WhatsApp. Finally, the workflow sends the AI-generated response back to the customer via WhatsApp.

## Output Details
The workflow sends an AI-generated response to the customer via WhatsApp.
