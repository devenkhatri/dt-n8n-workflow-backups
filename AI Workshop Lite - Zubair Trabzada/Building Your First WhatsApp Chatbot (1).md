# Workflow Analysis for WhatsApp Sales AI Agent with Product Catalogue

## Description
This workflow creates a WhatsApp chatbot powered by AI that helps customers navigate a 2024 product brochure for Yamaha Powered Loudspeakers. The chatbot uses a vector store built from the brochure to provide accurate, context-aware responses to user inquiries.

## Input Details
The workflow is triggered by incoming WhatsApp messages and receives message data including sender info and message content.

## Process Summary
First, a product brochure PDF is downloaded and its text extracted. This text is split into chunks and loaded into an in-memory vector store using OpenAI embeddings. When a WhatsApp message arrives, the workflow checks if it's a text message. Non-text messages receive an automated reply asking for text only. Text messages are sent to an AI Sales Agent powered by GPT-4o, which can access the product brochure vector store to answer customer questions accurately. The agent maintains conversation memory per user and responds with relevant information from the brochure.

## Output Details
The workflow sends AI-generated responses back to the WhatsApp user or a rejection message for non-text inputs.

## Tags
WhatsApp, AI Agent, Vector Store, Product Catalogue, Chatbot, OpenAI, GPT-4, Embeddings, Customer Support, Sales Assistant
