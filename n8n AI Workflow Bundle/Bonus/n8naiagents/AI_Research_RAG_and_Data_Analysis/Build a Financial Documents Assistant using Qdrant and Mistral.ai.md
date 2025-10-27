# Workflow Analysis for Financial Documents Assistant with Qdrant and Mistral.ai

## Description
This workflow creates an AI assistant to analyze financial documents using Qdrant for vector search and Mistral.ai for natural language understanding and generation. It allows users to upload documents, vectorize their content, store them, and answer questions based on the document content.

## Input Details
The workflow is triggered manually and receives a document path and a user query as input.

## Process Summary
The workflow starts by retrieving document content from Google Drive, splitting it into manageable chunks, and generating embeddings for each chunk using Cohere. These embeddings are then stored in Qdrant. Subsequently, the workflow takes a user query, generates an embedding for it, searches for relevant document chunks in Qdrant, and finally uses Mistral.ai to generate an answer based on the retrieved information and the user's query.

## Output Details
The workflow outputs a natural language answer from Mistral.ai based on the financial document content.
