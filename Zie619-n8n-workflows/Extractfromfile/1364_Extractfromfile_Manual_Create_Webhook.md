# Workflow Analysis for WhatsApp Sales AI Agent with Product Catalog

## Description
This workflow creates a WhatsApp chatbot powered by AI that helps customers navigate a 2024 Yamaha Powered Loudspeakers product brochure. It uses a vector store built from the brochure PDF to answer user questions accurately and sends responses directly back over WhatsApp.

## Input Details
The workflow is triggered by incoming WhatsApp messages and also includes a manual trigger to initialize the product catalog vector store from a remote PDF.

## Process Summary
First, the workflow downloads a product brochure PDF via HTTP request and extracts its text content. The text is split into chunks, embedded using OpenAI, and stored in an in-memory vector store to create a searchable knowledge base. When a WhatsApp message arrives, the workflow checks if it's a text message; non-text messages receive an error reply. Valid text messages are sent to an AI agent (GPT-4o) with access to the product catalog vector store and conversation memory. The agent generates a context-aware response based on the brochure content, which is then sent back to the user via WhatsApp.

## Output Details
The workflow sends personalized, AI-generated text responses to WhatsApp users based on the product brochure knowledge base, or a fallback message for unsupported message types.

## Tags
WhatsApp, AI agent, vector store, OpenAI, product catalog, chatbot, PDF processing, embeddings, GPT-4, customer support
