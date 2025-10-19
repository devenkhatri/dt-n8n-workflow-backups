# Workflow Analysis for WhatsApp AI-Powered RAG Chatbot with OpenAI

## Description
This workflow creates a comprehensive WhatsApp AI-powered chatbot leveraging OpenAI for Retrieval Augmented Generation (RAG) to provide intelligent responses.

## Input Details
The workflow is triggered by an incoming WhatsApp message via a webhook.

## Process Summary
The workflow receives a WhatsApp message and extracts relevant information. It then uses OpenAI to generate an embedding for the message and searches a Pinecone vector database for relevant context. This context is then used with OpenAI to generate a natural language response. Finally, the response is translated optionally and sent back to the user via WhatsApp.

## Output Details
The workflow sends an AI-generated, context-aware response back to the user on WhatsApp.
