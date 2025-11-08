# Workflow Analysis for Pinecone AI Assistant with Document Ingestion

## Description
This workflow provides an AI assistant powered by Pinecone for answering questions about earnings reports and includes a separate mechanism to ingest PDF documents into a vector database for knowledge base expansion.

## Input Details
The workflow is triggered by either a chat message for AI assistance or a form submission containing a PDF file for document ingestion.

## Process Summary
The workflow operates in two main modes: 1. AI Assistant Mode: Upon receiving a chat message, an AI agent utilizes an OpenRouter Chat Model, equipped with a Pinecone tool to search earnings reports and a calculator. It processes the query, retrieves information, and formulates a response, citing sources. 2. Document Ingestion Mode: When a PDF is submitted via a form, the workflow loads the document, generates OpenAI embeddings, and stores them in either a Pinecone or Supabase vector store, updating the knowledge base.

## Output Details
For chat messages, the workflow outputs a generated AI response with citations. For form submissions, it updates either the Pinecone or Supabase vector databases with new document embeddings.
