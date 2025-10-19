# Workflow Analysis for RAG Chatbot for Movie Recommendations

## Description
This workflow demonstrates a RAG (Retrieval-Augmented Generation) chatbot for movie recommendations using Qdrant for vector search and OpenAI for natural language processing.

## Input Details
The workflow is manually triggered or can be triggered via a webhook or API call.

## Process Summary
The workflow starts by clearing the chat history for a fresh interaction. Then, it defines the persona and instructions for the chatbot. It generates an embedding for the user's message using OpenAI and searches a Qdrant vector database for relevant movie information. The retrieved context is then combined with the user's message and sent to OpenAI to generate a movie recommendation. Finally, the generated response is saved to the chat history.

## Output Details
The workflow outputs a movie recommendation as a chat response, which is then stored in the chat history.
