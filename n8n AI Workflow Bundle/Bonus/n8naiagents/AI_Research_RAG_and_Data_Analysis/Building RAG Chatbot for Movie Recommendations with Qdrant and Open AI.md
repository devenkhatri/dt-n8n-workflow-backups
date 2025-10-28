# Workflow Analysis for Movie Recommendation RAG Chatbot with Qdrant Vector Store and OpenAI

## Description
This workflow builds a vector database of IMDB movie descriptions using OpenAI embeddings and Qdrant, then serves a chat‑based recommender that takes a user's positive and negative preferences, queries the vector store, and returns the top three movie suggestions.

## Input Details
Data is triggered either by a manual test run that pulls a CSV from GitHub, or by a chat webhook that receives a user message containing positive and negative movie preferences.

## Process Summary
1) The manual trigger fetches the Top_1000_IMDB_movies.csv from GitHub, extracts each row, creates document metadata, splits the text, generates OpenAI embeddings, and inserts them into the Qdrant collection "imdb". 2) When a chat message arrives, an AI Agent with a system prompt handles the request and invokes the "movie_recommender" tool (which executes the same workflow). 3) The tool embeds the positive and negative example texts via OpenAI, merges the embeddings, and calls Qdrant's recommendation API to retrieve the three most similar movies. 4) It then fetches the full payload for those movie IDs, selects relevant fields (name, description, release year, score), aggregates them, and returns the list to the AI Agent. 5) The agent formats a friendly response with the recommended movies and sends it back through the chat webhook.

## Output Details
The workflow sends a chat response containing the names and descriptions of the top three recommended movies to the user.
