# Workflow Analysis for Automated Survey Insights with Qdrant

## Description
This workflow automates the analysis of survey responses, extracts key insights, and stores them in Qdrant for easy retrieval.

## Input Details
This workflow starts manually, receiving JSON survey data as input.

## Process Summary
The workflow processes an array of survey responses, converting each into a JSON object. For each response, it generates an embedding, identifies key insights, and creates a title. Finally, it formats the extracted insights and stores them, along with their embeddings and titles, in the Qdrant vector database.

## Output Details
The workflow outputs the processed insights and stores them in the Qdrant vector database for future querying.
