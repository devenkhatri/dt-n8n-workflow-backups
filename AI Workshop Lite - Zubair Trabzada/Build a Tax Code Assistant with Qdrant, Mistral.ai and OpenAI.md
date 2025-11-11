# Workflow Analysis for Texas Tax Code AI Assistant

## Description
This workflow creates an AI-powered legal assistant that answers questions about Texas state tax codes by downloading official tax code PDFs, extracting and organizing them into structured sections, storing them in a Qdrant vector database with Mistral.ai embeddings, and enabling natural language queries through an AI agent with specialized search tools.

## Input Details
The workflow is triggered manually to ingest tax code data, and also accepts user chat messages via a webhook for querying the tax code knowledge base.

## Process Summary
First, the workflow downloads a ZIP file containing Texas tax code PDFs, extracts them, and parses each PDF into structured chapters and sections. It then chunks the content, generates Mistral embeddings, and stores the data in a Qdrant vector store with metadata. For user queries, an AI agent uses two tools: one to search relevant sections via vector similarity, and another to retrieve full sections by chapter or section number using Qdrant's filtering capabilities.

## Output Details
The workflow returns formatted responses to user queries either as summarized answers with source references or as full retrieved tax code sections, delivered through the chat interface.

## Tags
AI assistant, tax code, legal assistant, Qdrant, Mistral embeddings, PDF processing, vector database, AI agent, document parsing, RAG
