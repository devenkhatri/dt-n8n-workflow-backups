# Workflow Analysis for Building RAG Chatbot for Movie Recommendations with Qdrant and Open AI

## Description
This workflow creates a Retrieval-Augmented Generation (RAG) chatbot that recommends movies based on user preferences. It uses a dataset of top IMDB movies, stores their descriptions as vector embeddings in Qdrant, and leverages OpenAI to understand user requests and generate personalized movie suggestions.

## Input Details
The workflow is triggered either manually (for data ingestion) or via a chat message containing positive and/or negative movie preferences.

## Process Summary
First, movie data is fetched from a GitHub-hosted CSV file, parsed, and loaded into Qdrant as vector embeddings using OpenAI's embedding model. When a user sends a chat message, the AI agent interprets the request and invokes a tool that processes positive and negative examples by converting them into embeddings via OpenAI. These embeddings are then used to query Qdrant's recommendation API to find the top 3 similar movies. The workflow retrieves the movie metadata from Qdrant and formats it for the AI agent to present as a natural language response.

## Output Details
The workflow outputs a chat response with the top 3 recommended movies based on the user's preferences, delivered through the AI agent interface.

## Tags
RAG, movie recommendation, Qdrant, OpenAI, chatbot, vector database, embeddings, AI agent
