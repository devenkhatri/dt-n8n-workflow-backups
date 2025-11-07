# Workflow Analysis for RAG Pipeline and Chatbot for Google Drive FAQs

## Description
This workflow automates the process of building a Retrieval-Augmented Generation (RAG) knowledge base from Google Drive documents and powers an AI chatbot that uses this knowledge base to answer user queries.

## Input Details
The workflow is triggered either when a new file is created in a specified Google Drive folder or when a chat message is received.

## Process Summary
Upon a new file creation in Google Drive, the workflow downloads the file, loads its content, and splits it into manageable text chunks. These text chunks are then converted into numerical vector embeddings using OpenAI. The generated embeddings are stored in a Pinecone vector database, forming the RAG knowledge base for FAQs. Separately, when a chat message is received, an AI Agent powered by an OpenRouter chat model is activated. This AI agent utilizes a configured tool that queries the Pinecone vector store (knowledge base) to retrieve relevant information based on the chat message, enabling informed responses.

## Output Details
The RAG pipeline populates and updates a Pinecone vector database, while the chatbot generates and returns intelligent responses to incoming chat messages based on the stored knowledge.
