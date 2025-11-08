# Workflow Analysis for RAG Document Management and Chatbot

## Description
This workflow automates the management of a knowledge base by processing documents from Google Drive and storing their searchable content (embeddings) in Supabase. It also provides an AI chatbot that can answer questions by retrieving information from these documents.

## Input Details
The workflow is triggered by file creation, update, or deletion events in specific Google Drive folders, or by incoming chat messages for the AI agent.

## Process Summary
When a new file is created in Google Drive, it is downloaded, processed, embedded using OpenAI, and stored in a Supabase vector database. If an existing file is updated, its old record is deleted, and the new version is processed and re-inserted into Supabase. If a file is moved to the recycling bin, its corresponding entry is removed from Supabase. For chat messages, an AI agent uses an OpenRouter chat model and retrieves information from the Supabase vector store via OpenAI embeddings to formulate responses.

## Output Details
The workflow maintains an accurate and up-to-date knowledge base of document embeddings in Supabase and provides intelligent, document-informed responses to user chat queries.
