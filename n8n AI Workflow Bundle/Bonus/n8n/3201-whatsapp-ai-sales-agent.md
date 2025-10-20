# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI, providing instant responses and lead qualification to enhance sales efficiency and customer satisfaction.

## Input Details
The workflow is triggered by an incoming message on WhatsApp via a webhook.

## Process Summary
The workflow first checks for existing customer history in HubSpot. If found, it retrieves the conversation history; otherwise, it creates a new contact. It then uses an AI model to generate a sales-oriented response based on the customer's message and conversation history. Finally, it sends the AI-generated message back to the customer on WhatsApp and updates the conversation history in HubSpot.

## Output Details
The workflow sends AI-generated sales messages to customers on WhatsApp and updates communication logs in HubSpot.
