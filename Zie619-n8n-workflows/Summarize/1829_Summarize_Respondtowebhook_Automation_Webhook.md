# Workflow Analysis for Adaptive RAG

## Description
This n8n workflow implements an Adaptive Retrieval-Augmented Generation (RAG) approach to classify user queries and apply different retrieval and generation strategies based on the query type (Factual, Analytical, Opinion, or Contextual). It aims to provide more relevant and tailored answers from a knowledge base stored in a Qdrant vector store. This workflow is optimized for production use with comprehensive error handling, security, and documentation.

## Input Details
The workflow is triggered either by a chat interface via a webhook or by another n8n workflow, receiving a user query, a chat memory key for conversation history, and a vector store ID specifying the Qdrant collection.

## Process Summary
First, the workflow standardizes the incoming user query, chat memory key, and vector store ID. Next, a Google Gemini agent classifies the user query into one of four categories: Factual, Analytical, Opinion, or Contextual. Based on this classification, the workflow routes to a specific strategy where another Gemini agent adapts the query (e.g., for precision, sub-questions, diverse perspectives, or implied context). Subsequently, the adapted query is used to retrieve relevant documents from a Qdrant vector store, and their content is concatenated. Finally, a Google Gemini agent generates a comprehensive answer using a tailored system prompt, the retrieved context, the original query, and chat history.

## Output Details
The workflow produces a generated answer which is sent back to the user as a webhook response.

## Tags
automation,n8n,production-ready,excellent,optimized
