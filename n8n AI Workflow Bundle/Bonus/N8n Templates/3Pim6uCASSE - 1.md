# Workflow Analysis for Firecrawl AI Search Agent

## Description
This workflow demonstrates how to use the Firecrawl /search API endpoint with an AI agent to convert natural language queries into structured search requests. It showcases various search operators and returns comprehensive search results.

## Input Details
The workflow is triggered by receiving a chat message, which serves as the natural language input for the search query.

## Process Summary
1. A chat message initiates the workflow, providing a natural language search request. 2. An AI Search Agent, powered by a language model (GPT 4.1 mini), interprets the chat message. 3. The agent converts the natural language instruction into a structured Firecrawl search query, applying appropriate operators like site:, inurl:, or exclusion terms. 4. It then calls the Firecrawl Search tool, sending the constructed query along with a specified or default limit (5) for results. 5. The Firecrawl Search tool executes an HTTP POST request to the Firecrawl API, requesting search results formatted as markdown and full-page screenshots.

## Output Details
The workflow outputs detailed search results obtained from the Firecrawl API, including titles, URLs, and other data fields for each search item.
