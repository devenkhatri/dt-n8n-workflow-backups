# Workflow Analysis for AI Chatbot with Memory

## Description
This workflow creates an AI chatbot with conversation memory using OpenAI embeddings and Pinecone to store and retrieve past conversations.

## Input Details
The workflow is triggered by an HTTP request containing a user message and a session ID.

## Process Summary
The workflow starts by receiving a user message and session ID. It then checks Pinecone for existing conversational context. If context exists, it retrieves and combines it with the current message. The combined message is then sent to OpenAI for generating a chatbot response, which is then stored in Pinecone along with the current session ID to maintain conversation memory.

## Output Details
The workflow returns the chatbot's response as an HTTP response.
