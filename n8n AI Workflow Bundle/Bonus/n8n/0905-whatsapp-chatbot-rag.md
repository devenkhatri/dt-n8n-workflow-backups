# Workflow Analysis for WhatsApp Chatbot with RAG

## Description
This workflow automates a WhatsApp chatbot that uses Retrieval Augmented Generation (RAG) to answer user queries using a knowledge base. It can also route specific queries to a human agent.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by extracting the user's message and phone number. It then retrieves relevant information from a knowledge base using a vector store (Pinecone) and generates a response using a large language model (LLM). If the query is related to human agent assistance, it creates a ticket in a CRM (Gohighlevel) and notifies the user. Otherwise, it sends the AI-generated response back to the user on WhatsApp.

## Output Details
The workflow sends automated AI-generated responses or human agent notifications back to the user on WhatsApp and optionally creates CRM tickets.
