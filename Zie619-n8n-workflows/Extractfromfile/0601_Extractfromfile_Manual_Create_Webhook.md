# Workflow Analysis for WhatsApp Sales AI Agent with Product Catalog

## Description
This workflow creates a WhatsApp chatbot powered by AI that helps customers navigate a product catalog (specifically Yamaha Powered Loudspeakers 2024) by answering their questions using a knowledge base built from a product brochure PDF.

## Input Details
The workflow is triggered by incoming WhatsApp messages and also includes a manual trigger to initially load and process the product brochure PDF from a provided URL.

## Process Summary
First, the workflow downloads a product brochure PDF via HTTP request and extracts its text content. This text is split into chunks, converted into vector embeddings using OpenAI, and stored in an in-memory vector database to create a searchable knowledge base. When a WhatsApp message is received, the workflow checks if it's a text message; non-text messages receive an automated reply asking for text-only input. Valid text messages are sent to an AI agent (using GPT-4o) which uses the vector store to retrieve relevant product information and generate informed responses, while maintaining conversation memory per user.

## Output Details
The workflow sends AI-generated responses back to the WhatsApp user via the WhatsApp API, providing answers based on the product brochure knowledge base.

## Tags
WhatsApp, AI Agent, Vector Store, OpenAI, Product Catalog, Chatbot, PDF Processing, Customer Support, n8n
