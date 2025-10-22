# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent, allowing businesses to respond to customer queries, provide product information, and manage sales inquiries efficiently.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow receives a WhatsApp message and then identifies if it is a new conversation or a continuation of an existing one. If it is a new conversation, it calls an AI model to generate a welcome message and initiates a new conversation thread. For existing conversations, it retrieves the conversation history, calls the AI model to generate a response based on the history and the new message, and then updates the conversation history. Before responding, it checks if it should call an external tool like a product catalog to resolve the query. Finally, it sends the AI-generated response back to the customer via WhatsApp.

## Output Details
The workflow sends AI-generated responses back to the customer on WhatsApp, maintaining an ongoing conversation.
