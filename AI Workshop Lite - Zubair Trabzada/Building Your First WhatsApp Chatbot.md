# Workflow Analysis for WhatsApp Sales AI Agent with Product Catalog

## Description
This workflow creates a WhatsApp chatbot powered by AI that helps customers navigate a product catalog (Yamaha Powered Loudspeakers 2024 brochure). The bot uses a vector store built from the brochure to provide accurate, context-aware responses to customer inquiries.

## Input Details
The workflow is triggered by incoming WhatsApp messages, specifically processing only text messages while rejecting other media types.

## Process Summary
First, the workflow sets up a product knowledge base by downloading a PDF brochure, extracting its text, splitting it into chunks, and storing embeddings in an in-memory vector store. When a text message arrives via WhatsApp, it's routed to an AI agent that uses the vector store to retrieve relevant product information. The AI agent maintains conversation memory per user and generates responses based on the brochure content. Non-text messages trigger an automated reply asking for text-only input. Finally, the AI's response is sent back to the user via WhatsApp.

## Output Details
The workflow sends AI-generated responses back to WhatsApp users, providing product information from the 2024 Yamaha brochure based on their questions.

## Tags
WhatsApp, AI Agent, Vector Store, Product Catalog, Customer Support, Chatbot, OpenAI, Embeddings, Sales Assistant
