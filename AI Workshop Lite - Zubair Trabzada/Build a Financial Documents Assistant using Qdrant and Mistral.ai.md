# Workflow Analysis for Financial Documents Assistant with Qdrant and Mistral.ai

## Description
This workflow creates a financial documents assistant that leverages AI models from Mistral.ai and a vector database (Qdrant) to provide intelligent responses to user queries.

## Input Details
The workflow is triggered by an HTTP request, receiving a question and a chat history as input.

## Process Summary
First, the workflow embeds the incoming question using a Mistral.ai model. Next, it queries a Qdrant vector database to find relevant documents based on this embedding. Then, it constructs a prompt incorporating the retrieved document information, the user's question, and the chat history. Finally, it uses another Mistral.ai model to generate a natural language answer to the query.

## Output Details
The workflow returns a JSON object containing the AI-generated answer to the user's financial document question.
