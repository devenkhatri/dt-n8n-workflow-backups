# Workflow Analysis for RAG AI Agent with Milvus and Cohere

## Description
This workflow implements a Retrieval-Augmented Generation (RAG) AI system that automatically processes new PDF files added to a Google Drive folder, converts them into searchable vector embeddings using Cohere, stores them in a Milvus vector database, and enables an AI chat agent to answer user queries based on the document content.

## Input Details
The workflow is triggered by two inputs: new PDF files uploaded to a specific Google Drive folder and incoming chat messages via a webhook.

## Process Summary
When a new file is added to the monitored Google Drive folder, it is downloaded and extracted for text content. The text is split into chunks, converted into vector embeddings using Cohere's multilingual model, and inserted into a Milvus vector database. Separately, when a chat message is received, the system uses the user's query to retrieve relevant document chunks from Milvus, then passes this context along with the query to an OpenAI GPT-4o model to generate an informed response, using a memory buffer to maintain conversation context.

## Output Details
The workflow enables a chat interface that returns AI-generated answers based on the content of uploaded documents, with document embeddings stored in Milvus for fast retrieval.

## Tags
RAG, AI agent, Milvus, Cohere, OpenAI, Google Drive, vector database, document processing, chatbot, embeddings, n8n, production-ready
