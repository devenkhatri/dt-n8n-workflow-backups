# Workflow Analysis for Customer Feedback Analysis with Qdrant and Information Extraction

## Description
This workflow processes customer feedback, extracts key information using AI, and stores it in Qdrant for similarity search and analysis. It enables businesses to gain insights from customer reviews and quickly identify trends or common issues.

## Input Details
The workflow is manually triggered and receives customer feedback as input, specifically customer reviews.

## Process Summary
The workflow starts by preparing the customer review data. Then, it uses an AI model to extract specific information from each review, such as sentiment and key topics. This extracted information, along with the original review, is then vectorized and stored in a Qdrant database, allowing for efficient similarity searches and data retrieval.

## Output Details
The workflow stores processed customer feedback, including extracted insights and vectors, into a Qdrant vector database, enabling further analysis and similarity searches.
