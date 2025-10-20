# Workflow Analysis for Adaptive RAG Strategy for Document Q&A

## Description
This workflow implements an adaptive RAG (Retrieval Augmented Generation) strategy to answer questions based on an uploaded document. It dynamically decides whether to use a basic RAG approach or a more advanced "HyDE" (Hypothetical Document Embeddings) strategy to retrieve relevant information before generating an answer.

## Input Details
The workflow is triggered manually and requires a document file (PDF or DOCX) and a user question as input.

## Process Summary
The workflow starts by uploading a document and a question. It then determines the best RAG strategy (basic or HyDE). If HyDE is chosen, it generates a hypothetical answer to improve retrieval. It queries a vector store for relevant document chunks. Finally, it uses the retrieved chunks and the original question to generate a comprehensive answer.

## Output Details
The workflow outputs the generated answer to the user.
