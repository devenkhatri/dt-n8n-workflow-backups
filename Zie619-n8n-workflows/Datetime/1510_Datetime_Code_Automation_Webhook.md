# Workflow Analysis for Intelligent Web Query and Semantic Re-Ranking Flow

## Description
This workflow automatically processes a user's research question by first generating an optimized web search query, fetching real-time search results using the Brave Search API, and then using AI to rank the top 10 most relevant results and extract useful information from them. The final ranked results and extracted insights are returned via a webhook response.

## Input Details
The workflow is triggered by a webhook that receives a 'Research Question' as input.

## Process Summary
1. A webhook receives the user's research question. 2. An AI model generates an optimized, time-aware search query based on the question. 3. The workflow sends this query to the Brave Search API to fetch web results. 4. The raw results are processed into a combined text format. 5. Another AI model semantically re-ranks the top 10 results, extracts relevant information, and structures the output in JSON format.

## Output Details
The workflow returns a JSON response via the webhook containing the top 10 ranked URLs (with title, link, and description) and any relevant information extracted from the search results.

## Tags
web search, semantic ranking, AI query generation, Brave API, webhook, automation, research assistant, LLM, n8n, production-ready
