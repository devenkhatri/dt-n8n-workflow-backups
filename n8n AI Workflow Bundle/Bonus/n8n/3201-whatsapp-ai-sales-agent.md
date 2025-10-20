# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent to answer questions, recommend products, and handle sales inquiries.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, the workflow extracts the incoming message and sender information from the webhook. Next, it sends the message to an AI assistant (OpenAI Chat) which determines the appropriate response based on the conversation history and predefined sales prompts. Then, the workflow formats the AI-generated response. Finally, the workflow sends the AI-generated response back to the customer on WhatsApp. If the AI detects an issue or needs to transfer to a human, it will escalate the conversation.

## Output Details
The workflow sends automated AI-generated responses or escalates to a human agent via WhatsApp to the customer.
