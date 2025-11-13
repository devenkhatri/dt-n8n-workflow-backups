# Workflow Analysis for Local File Trigger Workflow

## Description
This workflow automates the synchronization of local file system changes with a Qdrant vector store and enables an AI-powered Question & Answer agent to provide insights from the indexed documents using Mistral AI.

## Input Details
The workflow is triggered by changes (additions, modifications, deletions) in a specified local file directory (`/home/node/host_mount/local_file_search`) or can be initiated manually, receiving file event details.

## Process Summary
The workflow monitors a local folder for file events (add, change, delete). Upon a file event, it identifies the type of event and sets relevant variables. For deleted or changed files, it first searches for and removes existing vector points in the Qdrant collection. For newly added or modified files, it reads the file content, prepares it with metadata, generates embeddings using Mistral AI, and then stores these embeddings in the Qdrant vector store. Separately, a chat trigger activates a Question and Answer chain that uses Mistral AI as the chat model and Qdrant as a vector store retriever to answer user queries based on the indexed files.

## Output Details
The workflow maintains an up-to-date Qdrant vector store with file embeddings and offers an AI agent that provides answers to questions based on the content of the synchronized documents.

## Tags
file synchronization, Qdrant, vector store, Mistral AI, RAG, AI agent, document processing, local file trigger, automation
