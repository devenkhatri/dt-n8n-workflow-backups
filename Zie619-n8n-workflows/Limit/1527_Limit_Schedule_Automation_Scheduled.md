# Workflow Analysis for RAG on living data

## Description
This workflow automates the process of keeping a knowledge base up-to-date and using it for question answering. It regularly fetches updated documents from Notion, processes them to create embeddings, and stores these embeddings in a Supabase vector database. Additionally, it provides a chatbot interface for users to ask questions, which are then answered using the knowledge stored in the vector database.

## Input Details
The workflow receives updated Notion pages from a specified "Knowledge Base" database on a minute-by-minute schedule, and also takes user questions via a chat message trigger.

## Process Summary
1. The workflow is triggered every minute to check for recently updated pages in a Notion "Knowledge Base" database.
2. For each updated page, any old embeddings associated with that page are deleted from the Supabase vector store.
3. The content of the Notion page is retrieved, combined into a single text, and then split into smaller chunks.
4. OpenAI generates vector embeddings for these text chunks, which are then stored in the Supabase "documents" vector store along with relevant metadata.
5. Separately, when a chat message is received, the message is processed by a Question and Answer Chain that retrieves relevant information from the Supabase vector store and uses an OpenAI Chat Model to formulate an answer.

## Output Details
The workflow continuously updates a Supabase vector database with new embeddings of Notion documents, and it provides natural language answers to user questions received via a chat interface.

## Tags
automation, n8n, production-ready, excellent, optimized, Notion, Supabase, OpenAI, RAG, Knowledge Base, Chatbot, Embeddings, Vector Store
