# Workflow Analysis for Automated PDF Processing for Pinecone Reservations

## Description
This workflow automates the extraction of text from PDF documents, processes it through OpenAI embeddings, splits the text into chunks, and stores the chunks in Pinecone for efficient searching and retrieval related to reservations.

## Input Details
This workflow is triggered manually and processes a single PDF file containing reservation information.

## Process Summary
The workflow starts by reading a PDF file and extracting its text content. It then uses OpenAI to create embeddings from the extracted text. The text is subsequently split into smaller chunks to prepare it for storage. Finally, these text chunks, along with their embeddings, are inserted into a Pinecone vector database for indexing and future retrieval.

## Output Details
The workflow stores processed text chunks and their corresponding embeddings in a Pinecone database, making the reservation information searchable and retrievable.
