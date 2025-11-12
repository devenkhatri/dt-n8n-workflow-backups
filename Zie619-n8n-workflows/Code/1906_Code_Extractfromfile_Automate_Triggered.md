# Workflow Analysis for Google Drive Automation

## Description
This workflow automatically processes new PDF files added to a specified Google Drive folder by extracting their text, cleaning it, generating vector embeddings, and storing them in a Pinecone vector database. It also supports answering user queries by retrieving relevant document chunks from Pinecone and generating AI-powered responses using contextual information.

## Input Details
The workflow is triggered by new files created in a specific Google Drive folder and also accepts user chat queries via a webhook trigger.

## Process Summary
When a new file is added to the monitored Google Drive folder, the workflow downloads it, extracts text if it's a PDF, and cleans the text by removing line breaks and special characters. The cleaned text is split into chunks, converted into embeddings using Google Gemini, and stored in a Pinecone vector index. Separately, when a user submits a chat query, the system generates an embedding for the query, retrieves the most relevant document chunks from Pinecone, constructs a contextual prompt, and sends it to an AI chat model (via OpenRouter) to generate a response.

## Output Details
The workflow stores processed document embeddings in Pinecone and generates AI-powered answers to user queries based on the indexed documents, which can be returned via webhook or used in a chat interface.

## Tags
Google Drive, PDF processing, RAG, Pinecone, vector embeddings, AI chat, automation, n8n, document indexing, OpenRouter
