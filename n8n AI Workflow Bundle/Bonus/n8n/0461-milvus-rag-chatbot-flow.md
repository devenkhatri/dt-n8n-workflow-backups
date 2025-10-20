# Workflow Analysis for Milvus RAG Chatbot Flow

## Description
This workflow demonstrates a chatbot that leverages Milvus for Retrieval Augmented Generation (RAG) to provide informative and contextually relevant responses.

## Input Details
The workflow is triggered by an HTTP request via a webhook, receiving user messages as input.

## Process Summary
The workflow begins by receiving a user message. It then encodes this message into an embedding using an OpenAI Text Embeddings node. This embedding is used to query a Milvus vector database, retrieving relevant documents based on semantic similarity. Finally, the retrieved information along with the user’s query is sent to an OpenAI Chat node to generate a comprehensive and contextually relevant response.

## Output Details
The workflow responds to the initial HTTP request with the AI-generated chatbot's answer.
