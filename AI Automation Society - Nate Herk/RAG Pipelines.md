# Workflow Analysis for RAG Pipelines

## Description
This workflow implements a Retrieval-Augmented Generation (RAG) system that automatically processes documents added to a Google Drive folder, converts them to embeddings, and stores them in a Supabase vector database. It also enables an AI chat agent to answer questions using the stored knowledge, and supports updating or deleting documents by watching for file changes or moves to a recycling bin folder.

## Input Details
The workflow is triggered by file events in specific Google Drive folders: new files, updated files, or files moved to a recycling bin folder, as well as incoming chat messages via a webhook.

## Process Summary
When a new file is added to the designated Google Drive folder, it is downloaded, converted to PDF if needed, split into documents, embedded using OpenAI, and stored in Supabase. When a file is updated, the old version is deleted from Supabase and the new version is processed and stored. When a file is moved to the recycling bin folder, its corresponding entries are deleted from Supabase. Separately, when a chat message is received, an AI agent uses the Supabase vector store as a retrieval tool to answer questions based on the stored documents.

## Output Details
The workflow populates and maintains a Supabase vector database with document embeddings and enables an AI chat agent to respond to user queries with relevant information retrieved from that database.

## Tags
RAG, Google Drive, Supabase, OpenAI, embeddings, vector store, document processing, AI agent, chatbot, file automation
