# Workflow Analysis for MongoDB Agent

## Description
This workflow functions as an AI autonomous agent powered by OpenAI and MongoDB. It is designed to process chat messages, query movie data from a MongoDB database using aggregation, and allows users to store their favorite movies back into the database.

## Input Details
The workflow is primarily triggered by chat messages received via a webhook, which serve as user input for the AI agent.

## Process Summary
The workflow receives chat messages and processes them through an AI Agent powered by an OpenAI chat model. The AI agent uses tools to interact with a MongoDB database, either by performing aggregation queries to retrieve movie context based on user requests (e.g., filtering by rating) or by calling a sub-workflow to insert a favorite movie title if confirmed by the user. A window buffer memory helps maintain conversational context throughout the interaction. The workflow also includes error handling for robust operation.

## Output Details
The workflow either returns movie recommendations and information based on MongoDB queries or records a user's favorite movie title by inserting it into the database.

## Tags
automation, n8n, production-ready, excellent, optimized, MongoDB, AI, OpenAI, Chatbot, Movie Recommendation
