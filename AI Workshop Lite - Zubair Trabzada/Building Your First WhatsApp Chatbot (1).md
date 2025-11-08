# Workflow Analysis for WhatsApp Sales AI Agent with Product Brochure Knowledgebase

## Description
This workflow sets up a WhatsApp chatbot that acts as a sales agent. It uses an AI model to answer customer questions by leveraging a product brochure as its knowledge base and maintaining conversation history.

## Input Details
The workflow is triggered by incoming WhatsApp messages, specifically text messages from customers, or can be manually initiated to set up the product catalog.

## Process Summary
First, the workflow downloads a product brochure PDF via an HTTP request, extracts its text content, splits it into smaller chunks, and embeds it to create an in-memory product catalog vector store. When a WhatsApp message is received, it checks if it is a text message; if not, it sends an apology. For text messages, an AI Sales Agent, equipped with conversational memory and access to the product catalog via a vector store tool, processes the user's query and generates a factual response. This agent leverages OpenAI models for its intelligence and embeddings.

## Output Details
The workflow sends a text message response back to the originating WhatsApp user, either providing information from the product catalog or indicating an inability to process non-text messages.
