# Workflow Analysis for Trustpilot Review Insights Generation

## Description
This workflow extracts reviews from Trustpilot for a specified company, vectors them in a Qdrant store, clusters similar opinions, and uses OpenAI to produce concise insights that are appended to a Google Sheet for business analysis.

## Input Details
Triggered manually; the company ID is set within the workflow before execution.

## Process Summary
When triggered, the workflow first clears existing review data from the Qdrant collection for the company. It then scrapes up to three pages of Trustpilot reviews, extracts and normalises the data, and stores each review as a document with embeddings in Qdrant. After embedding, K‑means clustering groups similar reviews, and clusters containing more than two reviews are selected. The payload of each cluster’s reviews is fetched and passed to an OpenAI chat model that summarises the cluster, determines overall sentiment, and suggests improvements. Finally, the insights along with metadata are appended to a pre‑configured Google Sheet.

## Output Details
Adds a row for each review cluster to a Google Sheet, containing the company ID, date range, number of responses, raw review excerpts, and the generated insight, sentiment, and improvement suggestions.
