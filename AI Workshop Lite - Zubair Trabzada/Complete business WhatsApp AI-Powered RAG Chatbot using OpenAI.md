# Workflow Analysis for Business WhatsApp AI RAG Chatbot

## Description
This workflow powers an AI chatbot for WhatsApp Business that answers customer inquiries using a Retrieval-Augmented Generation (RAG) system. It retrieves relevant information from a knowledge base stored in Google Drive, converts it into vector embeddings, and uses them to provide accurate, context-aware responses to users' messages.

## Input Details
The workflow is triggered by incoming WhatsApp messages via a POST webhook from Meta, and it also supports manual testing and setup via a manual trigger.

## Process Summary
First, the workflow verifies the WhatsApp webhook (GET) and processes incoming messages (POST). It checks if the payload contains a user message, then retrieves relevant documents from a Google Drive folder, converts them into text chunks, and stores their embeddings in a Qdrant vector database. When a user sends a message, the AI Agent uses these embeddings along with conversation memory and a configured system prompt to generate a contextual response using OpenAI's GPT-4o-mini model. Finally, the response is sent back to the user via WhatsApp.

## Output Details
The workflow sends AI-generated text responses back to the WhatsApp user who initiated the conversation.

## Tags
WhatsApp, AI Chatbot, RAG, Qdrant, Google Drive, OpenAI, Vector Store, LangChain, Customer Support, n8n
