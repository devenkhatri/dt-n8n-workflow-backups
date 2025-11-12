# Workflow Analysis for AI Agent to Chat With Files in Supabase Storage

## Description
This workflow automates the processing of files stored in Supabase by extracting their content, converting it into searchable vector embeddings, and enabling AI-powered chat interactions to retrieve relevant information from those files.

## Input Details
The workflow is triggered manually or via a chat message, and it fetches file metadata and content from a Supabase storage bucket.

## Process Summary
The workflow first retrieves a list of all files from Supabase storage and compares them against already processed files in a 'files' table to avoid duplicates. New or unprocessed files are downloaded, and their content is extracted based on file type (e.g., PDF or text). The extracted text is split into manageable chunks, converted into vector embeddings using OpenAI, and stored in a Supabase vector store along with file metadata. A separate AI agent flow allows users to query this vector store through a chat interface to retrieve relevant document snippets.

## Output Details
The workflow stores processed file metadata and vector embeddings in Supabase tables and enables an AI chatbot to respond to user queries using the indexed document content.

## Tags
AI, Supabase, file processing, vector embeddings, chatbot, OpenAI, document retrieval, automation, n8n, RAG
