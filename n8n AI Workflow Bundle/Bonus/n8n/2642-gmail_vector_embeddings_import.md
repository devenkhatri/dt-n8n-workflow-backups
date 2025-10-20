# Workflow Analysis for Gmail Email to Vector Database Import

## Description
This workflow extracts emails from Gmail, creates embeddings for their content, and imports these embeddings into a vector database for efficient search and retrieval.

## Input Details
This workflow is triggered manually and does not receive any input data.

## Process Summary
The workflow first retrieves the last 50 emails from the user's Gmail inbox. Each email's subject, sender, and body are then combined into a single text string. This combined text is then used to generate a vector embedding. Finally, the original email content along with its generated vector embedding is imported into a vector database.

## Output Details
The workflow outputs email subject, sender, body, and their corresponding vector embeddings into a Qdrant vector database.
