# Workflow Analysis for HelloFresh Recipe Recommendation AI with Qdrant and Mistral

## Description
This workflow fetches HelloFresh weekly menu data, processes it, and stores it in both a Qdrant vector store and a SQLite database. It then enables an AI agent, powered by Mistral AI, to recommend recipes based on user preferences (likes and dislikes) by leveraging Qdrant's advanced recommendation capabilities.

## Input Details
The workflow is triggered either manually to ingest and store HelloFresh menu data or via a chat interface when a user queries the AI agent for recipe recommendations, providing their preferences.

## Process Summary
The workflow first scrapes the current week's menu from the HelloFresh website and extracts detailed recipe information. This data is then prepared and simultaneously stored as vector embeddings in Qdrant and as full documents in a SQLite database. An AI agent is configured with Mistral AI and a custom tool to interact with the Qdrant recommendation engine. When the AI agent receives a user's positive and negative recipe preferences, it converts them into embeddings and queries Qdrant to find the best matching recipes from the current week's menu. Finally, it retrieves the full recipe details from the database and returns them as recommendations.

## Output Details
The workflow establishes a searchable database of HelloFresh recipes in Qdrant and SQLite, and through the AI agent, provides personalized recipe recommendations to the user via a chat interface.
