# Workflow Analysis for Document to Study Notes with AI and Vector Database

## Description
This workflow automates the process of converting documents into structured study notes using AI, storing them in a vector database for easy retrieval and querying. It leverages MistralAI for intelligent note generation and Qdrant for efficient vector storage and search.

## Input Details
The workflow is triggered manually and requires document text as input.

## Process Summary
The workflow starts by preparing the input document for processing. It then uses MistralAI to generate embedding vectors from the document content and stores these vectors, along with the document text, into Qdrant. Subsequently, it queries the Qdrant database to retrieve relevant information based on a user-defined prompt. Finally, it uses MistralAI again to refine the retrieved information into concise study notes, leveraging templating for structured output.

## Output Details
The workflow outputs AI-generated study notes based on the processed document and stored in Qdrant.
