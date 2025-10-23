# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI to answer questions, recommend products, and assist with purchases, improving customer service and sales efficiency.

## Input Details
The workflow is triggered by an incoming message to a WhatsApp business account.

## Process Summary
The workflow receives a WhatsApp message and extracts relevant information. It then uses an AI model (ChatGPT) to generate a response based on the customer's query. If the AI deems the conversation important for a human, it sends a notification to a Slack channel. Finally, the AI-generated response is sent back to the customer on WhatsApp.

## Output Details
The workflow sends AI-generated responses to customers on WhatsApp and can optionally send notifications to a Slack channel for important conversations.
