# Workflow Analysis for Document Q&A with Citations from Google Drive

## Description
This workflow allows users to ask questions about a document stored in Google Drive and receive answers with citations. It first ingests a specified Google Drive file, splits it into manageable chunks, and stores these chunks with their embeddings in a Pinecone vector database. Subsequently, users can interact with a chatbot, posing questions which are then used to retrieve relevant document chunks from Pinecone. An OpenAI language model processes these chunks and the user's question to generate an informed answer, complete with references to the original document's sections.

## Input Details
The workflow is triggered manually to set up and ingest a document from a specified Google Drive URL, and then by a chat webhook to receive user questions.

## Process Summary
The workflow has two main parts. First, a manual trigger initiates the process of fetching a document from a Google Drive URL, extracting metadata, splitting its content into chunks, generating embeddings for these chunks using OpenAI, and finally storing them in a Pinecone vector database. Second, a chat trigger initiates a query process where a user's question is used to retrieve the most relevant document chunks from Pinecone. These chunks are then used as context for an OpenAI chat model to generate an answer, which is parsed to extract the answer and relevant chunk indices.

## Output Details
The workflow outputs an AI-generated answer to the user's question, including specific citations (file name and line numbers) from the source document, returned via the chat webhook.
