# Workflow Analysis for Intelligent Web Query and Semantic Re-Ranking Flow

## Description
This workflow intelligently generates optimized search queries from user research questions, performs live web searches using the Brave Search API, and then uses AI to re-rank and extract the most relevant information from the results—returning a curated list of top URLs and insights.

## Input Details
The workflow is triggered by a webhook that receives a 'Research Question' parameter containing the user's query.

## Process Summary
First, the workflow receives a research question via a webhook. It uses the current date and the user’s question to generate an optimized search query using an AI-powered 'Query Maker' node. This query is sent to the Brave Search API to fetch live web results. The titles, URLs, and descriptions of these results are aggregated into a single text block. Finally, a semantic re-ranker AI analyzes, ranks the top 10 results, extracts relevant information, and structures the output in JSON format.

## Output Details
The workflow responds to the original webhook with a JSON object containing the top 10 ranked URLs (with title, link, and description) and any relevant information extracted from the results.

## Tags
web search, AI ranking, semantic search, Brave API, research automation, query optimization, LLM, webhook, n8n, production-ready
