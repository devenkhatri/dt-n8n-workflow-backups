# Workflow Analysis for Local File Search with Qdrant and Mistral AI

## Description
This workflow monitors a local folder for file changes (add, modify, delete), synchronizes those files with a Qdrant vector database using Mistral AI embeddings, and provides a chat interface to ask questions about the files using a Mistral AI language model.

## Input Details
The workflow is triggered by file system events (file added, changed, or deleted) in a specified local directory, or manually via a test button.

## Process Summary
The workflow first detects file system events in a monitored folder and categorizes them as add, change, or delete operations. For deleted files, it removes the corresponding vector from Qdrant. For changed files, it first deletes the existing vector and then reprocesses the updated file. For new or changed files, it reads the file content, generates embeddings using Mistral AI, and stores the vector along with metadata in Qdrant. Finally, it provides a chat interface that uses Mistral AI with Qdrant as a retriever to answer questions about the stored files.

## Output Details
The workflow maintains a synchronized vector database in Qdrant and provides an AI-powered chat interface that answers questions based on the content of files in the monitored folder.

## Tags
local file, Qdrant, Mistral AI, RAG, file monitoring, vector database, embeddings, AI chatbot
