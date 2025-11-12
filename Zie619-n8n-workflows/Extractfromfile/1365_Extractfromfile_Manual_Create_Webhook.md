# Workflow Analysis for WhatsApp Sales AI Agent with Product Catalog

## Description
This workflow creates a WhatsApp chatbot powered by AI that answers customer questions using a product catalog (Yamaha loudspeakers brochure) stored in a vector database. It automatically responds to text messages, while rejecting non-text messages with a friendly note.

## Input Details
The workflow is triggered by incoming WhatsApp messages and also includes a manual trigger for initial setup of the product catalog vector store.

## Process Summary
First, the workflow downloads a product brochure PDF via HTTP request and extracts its text content. This text is split into chunks, embedded using OpenAI, and stored in an in-memory vector store to create a searchable product knowledgebase. When a WhatsApp message arrives, the workflow checks if it's a text message. If not, it sends a reply asking for text only. If it is text, the message is sent to an AI agent (using GPT-4o) that uses the vector store to retrieve relevant product information and generate a helpful response. Finally, the AI's reply is sent back to the user via WhatsApp.

## Output Details
The workflow sends automated WhatsApp replies to users—either an AI-generated answer based on the product catalog or a message requesting only text input.

## Tags
WhatsApp, AI Agent, Vector Store, OpenAI, Chatbot, Sales Assistant, PDF Processing, Text Embeddings, Automation, n8n
