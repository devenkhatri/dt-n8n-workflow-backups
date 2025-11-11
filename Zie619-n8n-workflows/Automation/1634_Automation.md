# Workflow Analysis for Hello Fresh Recipe Recommendation Workflow

## Description
This workflow helps users find a suitable recipe from Hello Fresh's current week menu based on their preferences and dietary restrictions. It retrieves the latest recipe data, filters it according to user input (likes and dislikes), and recommends the best match using AI-powered embedding and search.

## Input Details
The workflow is triggered manually and receives user preferences (positives and negatives) via a chat interface or test execution input.

## Process Summary
The workflow starts with a manual trigger and fetches the current week's Hello Fresh recipes, either from a database or by scraping/parsing the website. It processes and stores recipe data in a SQLite database. Using Mistral Cloud, it generates embeddings for recipe content and user preferences. It then leverages Qdrant to find the best-matching recipes based on these embeddings. Finally, a Mistral large language model formats a user-friendly recommendation based on the matched recipe.

## Output Details
The workflow outputs a personalized recipe recommendation message to the user, based solely on the current week’s Hello Fresh menu.

## Tags
hello fresh, recipe recommendation, AI chatbot, Mistral AI, Qdrant, embeddings, SQLite, n8n workflow, food tech, meal planning
