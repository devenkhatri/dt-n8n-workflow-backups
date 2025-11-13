# Workflow Analysis for RAG on living data

## Description
This workflow automates the process of creating and utilizing a Retrieval Augmented Generation (RAG) system based on Notion data. It keeps the knowledge base updated and allows for context-aware question answering.

## Input Details
The workflow is triggered either by a minute-based schedule that checks for updated Notion database pages or by a chat message received through a webhook.

## Process Summary
First, for updated Notion pages, the workflow processes each page individually. It deletes any existing embeddings for that page in Supabase, then retrieves all the page blocks. The content is concatenated into a single string, split into smaller chunks, and then OpenAI embeddings are generated for each chunk. Finally, these embeddings, along with relevant metadata like the Notion ID and name, are stored in a Supabase vector database. Separately, when a chat message is received, the workflow retrieves relevant information from the Supabase vector store and uses an OpenAI chat model to generate a comprehensive answer based on the provided context and the user's question.

## Output Details
The workflow populates a Supabase vector database with Notion page embeddings and provides intelligent, context-aware answers to chat messages using the stored embeddings.

## Tags
automation,n8n,production-ready,excellent,optimized
