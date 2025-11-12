# Workflow Analysis for Prod: Notion to Vector Store - Dimension 768

## Description
This workflow automatically captures new pages added to a Notion database, extracts and cleans their textual content, generates vector embeddings using Google Gemini, and stores the embeddings along with metadata in a Pinecone vector database for search or AI retrieval purposes.

## Input Details
The workflow is triggered when a new page is added to a specific Notion database, polling every minute for changes.

## Process Summary
The workflow starts by detecting a new Notion page via a trigger node. It then retrieves all content blocks from the new page and filters out non-text elements like images or videos. The remaining text blocks are concatenated into a single content string. Metadata such as page ID, creation time, and title are extracted, and the text is sent to Google Gemini to generate 768-dimensional embeddings. Finally, the embeddings and associated metadata are inserted into a Pinecone vector store.

## Output Details
The workflow outputs vector embeddings and page metadata to a Pinecone vector database for downstream AI or search applications.

## Tags
Notion, Pinecone, Google Gemini, vector embeddings, automation, production-ready, text processing, RAG
