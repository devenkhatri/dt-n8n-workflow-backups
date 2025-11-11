# Workflow Analysis for PDF -> Pinecone

## Description
This workflow downloads a Google Doc file, processes its content into text chunks, generates vector embeddings using OpenAI, and stores them in a Pinecone vector database under a specified namespace for semantic search or retrieval-augmented applications.

## Input Details
The workflow is manually triggered and downloads a specific Google Doc file based on a hardcoded file ID.

## Process Summary
The workflow starts by manually triggering a download of a Google Doc file. The downloaded file is processed by a default data loader to extract its content. The extracted text is split into smaller chunks using a recursive character text splitter. OpenAI embeddings are generated for these text chunks. Finally, the embeddings and associated document data are stored in a Pinecone vector database within the 'customerSupport' namespace.

## Output Details
The workflow stores the embedded document chunks in a Pinecone vector store for later use in vector similarity searches or AI applications.

## Tags
PDF processing, Google Drive, Pinecone, OpenAI embeddings, vector database, document ingestion, text splitting, RAG
