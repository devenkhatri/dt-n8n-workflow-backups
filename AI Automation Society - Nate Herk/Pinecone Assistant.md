# Workflow Analysis for Pinecone Assistant

## Description
This workflow enables an AI-powered assistant that answers user questions by searching through a knowledge base of earnings reports (e.g., from Tesla, Nike, and Nvidia) stored in Pinecone or Supabase. It supports real-time chat interactions and also allows users to upload new PDF documents to update the knowledge base.

## Input Details
The workflow is triggered either by a chat message via a webhook or by a form submission containing a PDF file.

## Process Summary
When a chat message is received, the Pinecone Assistant agent uses an OpenRouter language model and accesses a Pinecone knowledge base via an HTTP request to retrieve relevant information and generate a response with source citations. Separately, when a PDF is uploaded via a form, the document is processed using a data loader and OpenAI embeddings, then stored in both Pinecone and Supabase vector databases. Alternative agents using Pinecone Vector Store and Supabase Vector Store are also configured for comparison or fallback retrieval methods.

## Output Details
The workflow sends AI-generated responses to chat queries with document citations and ingests uploaded PDFs into vector databases for future retrieval.

## Tags
AI assistant, Pinecone, Supabase, vector database, document ingestion, earnings reports, chatbot, RAG, OpenRouter, OpenAI embeddings
