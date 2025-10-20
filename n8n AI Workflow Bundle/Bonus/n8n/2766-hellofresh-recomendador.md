# Workflow Analysis for HelloFresh Meal Recommender

## Description
This workflow helps HelloFresh users discover new recipes based on their preferences by providing personalized recommendations.

## Input Details
The workflow is triggered manually by an HTTP request containing a user ID and a list of disliked ingredients.

## Process Summary
First, the workflow fetches a list of recipes from the HelloFresh API. Then, it retrieves the user's preferences, including their favorite recipes and dietary habits. It filters out disliked ingredients and previously liked or disliked recipes. Finally, it uses OpenAI to generate new recipe recommendations and stores the interaction data.

## Output Details
The workflow returns a list of recommended recipes to the user and logs the interaction data in a PostgreSQL database.
