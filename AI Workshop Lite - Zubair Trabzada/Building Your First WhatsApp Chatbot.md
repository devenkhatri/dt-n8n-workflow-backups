# Workflow Analysis for WhatsApp Sales AI Agent with Product Catalog Knowledge Base

## Description
This workflow creates an intelligent WhatsApp chatbot that acts as a sales agent. It is equipped with a knowledge base derived from a product brochure, allowing it to answer customer questions factually. The agent maintains conversation memory and filters out unsupported message types.

## Input Details
The workflow is primarily triggered by incoming WhatsApp text messages from users, but also includes a manual trigger to initialize or update the product catalog knowledge base.

## Process Summary
First, a product brochure PDF is downloaded and its text content is extracted, then processed and stored as embeddings in an in-memory vector store to build a knowledge base. When a WhatsApp message is received, the workflow checks if it's a text message; if not, it sends an error message. For text messages, an AI Sales Agent uses an OpenAI chat model, conversation memory, and a vector store tool to query the product catalog for relevant information. The AI agent processes the user's query and the retrieved information to generate an informed response. Finally, the agent's response is sent back to the user via WhatsApp.

## Output Details
The workflow sends text-based responses to the original WhatsApp sender, either providing information from the product catalog or indicating an inability to process non-text messages.
