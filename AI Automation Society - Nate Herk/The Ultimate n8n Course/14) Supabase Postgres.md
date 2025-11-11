# Workflow Analysis for RAG Agent with Supabase/Postgres Memory and Google Drive Document Ingestion

## Description
This workflow implements a Retrieval-Augmented Generation (RAG) chatbot that answers user questions using both conversation history stored in Postgres and relevant information retrieved from a Supabase vector database. It also includes a separate process to load documents from Google Drive, split their text, and store their embeddings in Supabase for use by the chatbot.

## Input Details
The workflow is triggered by incoming chat messages via a webhook and can also be manually triggered to ingest documents from Google Drive.

## Process Summary
When a chat message is received, it is processed by an AI agent that uses an OpenAI language model, retrieves relevant context from a Supabase vector store using OpenAI embeddings, and maintains conversation history in a Postgres database. Separately, when manually triggered, the workflow downloads a file from Google Drive, splits its text into chunks using a recursive character splitter, generates embeddings for those chunks via OpenAI, and stores them in the Supabase vector database for future retrieval during chat interactions.

## Output Details
The workflow sends AI-generated responses back to the chat interface and stores document embeddings in Supabase for retrieval during future conversations.

## Tags
RAG, chatbot, AI agent, Supabase, Postgres, vector store, embeddings, OpenAI, Google Drive, document ingestion, memory
