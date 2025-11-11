# Workflow Analysis for Trustpilot Reviews Analysis Workflow

## Description
This workflow scrapes Trustpilot reviews for a specified company, stores them in a vector database, groups similar reviews using clustering, and generates actionable insights using AI, which are then exported to a Google Sheet.

## Input Details
The workflow is manually triggered and requires a company ID (Trustpilot URL slug) to be set in the 'Set Variables' node.

## Process Summary
The workflow starts by clearing existing reviews for the specified company from the Qdrant vector store. It then scrapes the latest Trustpilot reviews, extracts key data like author, rating, and text, and stores each review as a vector in Qdrant. After storage, it triggers a subworkflow that fetches reviews within a specified date range (defaulting to the current month), applies K-means clustering to group similar reviews, and filters clusters with at least 3 reviews. For each valid cluster, it retrieves the full review data and uses an AI model to generate a summary insight, sentiment, and suggested improvements. Finally, these insights along with raw review data are appended to a Google Sheet.

## Output Details
The workflow outputs AI-generated insights, sentiment analysis, and raw review data for each cluster of similar Trustpilot reviews to a specified Google Sheet.

## Tags
Trustpilot, review analysis, sentiment analysis, clustering, vector database, Qdrant, OpenAI, Google Sheets, web scraping, AI insights
