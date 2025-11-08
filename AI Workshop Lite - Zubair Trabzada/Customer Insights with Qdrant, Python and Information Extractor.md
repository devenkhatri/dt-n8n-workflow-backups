# Workflow Analysis for AI-Powered Trustpilot Customer Review Insights

## Description
This workflow generates highly-detailed customer insights from Trustpilot reviews. Works best when dealing with a large number of reviews. It imports Trustpilot reviews and vectorises them in a Qdrant vector store. It then identifies clusters of popular topics in reviews using a K-means clustering algorithm. Each valid cluster is analysed and summarised by an LLM, and finally, the LLM response and cluster results are exported back into a Google Sheet.

## Input Details
The workflow is triggered manually and takes a companyId (e.g., a Trustpilot recognized domain) as its primary input to scrape reviews.

## Process Summary
The workflow starts manually, clears existing Qdrant records for a specified company, and then scrapes the most recent Trustpilot reviews for that company. Extracted review details are transformed and stored as vector embeddings in a Qdrant vector database. A sub-workflow is triggered to analyze these reviews: it retrieves relevant reviews for the current month from Qdrant. A K-means clustering algorithm is applied to group similar reviews based on their embeddings, and clusters with fewer than three reviews are filtered out. Finally, an OpenAI LLM analyzes the reviews within each significant cluster to generate insights, sentiment, and suggested improvements, which are then prepared for export.

## Output Details
The workflow produces summarized customer insights, sentiment analysis, suggested improvements, and raw review data, which are then appended to a specified Google Sheet.
