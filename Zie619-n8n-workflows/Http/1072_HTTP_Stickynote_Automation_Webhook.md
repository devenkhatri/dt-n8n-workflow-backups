# Workflow Analysis for Perplexity Researcher

## Description
This workflow leverages the Perplexity AI Sonar model to perform intelligent research based on a user-provided query. It formats the query with a detailed system prompt, sends it to the Perplexity API, and extracts the relevant response content for downstream use.

## Input Details
The workflow is triggered by another workflow and receives a user query via input data (e.g., fields like 'query', 'question', or 'Research Query').

## Process Summary
First, the workflow receives a query from a parent workflow. It then assigns a system prompt and the user query to structured variables. Next, it sends a POST request to the Perplexity AI API using the Sonar model with specific parameters like temperature, max tokens, and recency filters. The API response is parsed to extract the main message content from the model's output. Finally, the extracted content is prepared as the workflow’s output.

## Output Details
The workflow outputs the cleaned response content from Perplexity AI, which can be used by the calling workflow for further processing or presentation.

## Tags
AI research, Perplexity AI, workflow automation, API integration, content extraction, n8n
