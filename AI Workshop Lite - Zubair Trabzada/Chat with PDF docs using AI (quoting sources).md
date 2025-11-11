# Workflow Analysis for Chat with Google Drive File using Pinecone and OpenAI

## Description
This workflow enables users to chat with a document stored in Google Drive by first ingesting it into a Pinecone vector database and then using OpenAI's language and embeddings models to answer questions with cited sources from the document.

## Input Details
The workflow has two entry points: a manual trigger to ingest a Google Drive file into Pinecone, and a chat trigger that accepts user questions via a webhook.

## Process Summary
First, a Bitcoin whitepaper file is downloaded from Google Drive, enriched with metadata, split into text chunks, and stored in Pinecone with OpenAI embeddings. When a user asks a question via the chat interface, the workflow retrieves the most relevant chunks from Pinecone using OpenAI embeddings, constructs a contextual prompt, and sends it to OpenAI's chat model. The model generates an answer along with citations, which are formatted to show the source file and line numbers before being returned as the final response.

## Output Details
The workflow returns a chat response containing the answer to the user's question and formatted citations indicating which parts of the source document were used.

## Tags
chat, pinecone, openai, google drive, embeddings, vector database, document qa, citations
