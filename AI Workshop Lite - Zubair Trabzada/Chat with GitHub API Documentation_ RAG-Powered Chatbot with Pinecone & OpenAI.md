# Workflow Analysis for Chat with GitHub OpenAPI Specification using RAG (Pinecone and OpenAI)

## Description
This workflow enables users to chat with a bot that answers questions about the GitHub REST API by using Retrieval-Augmented Generation (RAG). It fetches the official OpenAPI specification, stores it in a Pinecone vector database using OpenAI embeddings, and uses GPT-4o-mini to generate contextual responses based on user queries.

## Input Details
The workflow is triggered either manually (for indexing the GitHub OpenAPI spec) or via a chat message webhook (for user queries).

## Process Summary
First, the workflow fetches the GitHub OpenAPI specification JSON file from a public URL. It then splits the document into smaller chunks, generates OpenAI embeddings for each chunk, and stores them in a Pinecone vector database. When a user sends a chat message, the workflow generates an embedding for the query, retrieves relevant API documentation chunks from Pinecone, and uses GPT-4o-mini with memory context to generate a helpful response based on the retrieved information.

## Output Details
The workflow returns natural language responses to user queries about the GitHub API via the chat interface, using relevant excerpts from the official OpenAPI specification.

## Tags
RAG, chatbot, GitHub API, OpenAPI, Pinecone, OpenAI, embeddings, vector database, n8n, AI assistant
