# Workflow Analysis for Local File Synchronization and AI Q&A Workflow

## Description
This workflow continuously monitors a local file directory for changes, ensuring that a Qdrant vector database is synchronized with the file contents. It also enables an AI question-answering agent, powered by Mistral AI, to respond to queries based on the documents stored in Qdrant.

## Input Details
The workflow is triggered either manually or automatically when files are added, changed, or deleted within a specified local directory (`/home/node/host_mount/local_file_search`). It also has a chat trigger for AI Q&A.

## Process Summary
Upon a file system event (add, change, delete), the workflow determines the event type. If a file is deleted or changed, it first searches for and removes any existing vector representations of that file in the Qdrant database. If a file is added or changed, its content is read, prepared as a document, and split into chunks. Mistral AI generates embeddings for these chunks, which are then stored in the Qdrant vector database along with relevant metadata. Separately, a chat trigger initiates an AI question-answering process, where user questions are processed by a Mistral AI model that retrieves context from the Qdrant vector store to formulate responses.

## Output Details
The workflow maintains a synchronized Qdrant vector database with the latest document embeddings and provides AI-generated answers to user questions via a chat interface.

## Tags
file synchronization, Qdrant, Mistral AI, RAG, AI agent, document processing, local file trigger, vector database, embeddings, chat bot
