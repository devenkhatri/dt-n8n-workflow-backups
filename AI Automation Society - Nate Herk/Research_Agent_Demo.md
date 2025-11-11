# Workflow Analysis for Research Agent Demo

## Description
This workflow acts as an AI-powered research assistant that answers user queries by intelligently searching through Wikipedia, Hacker News, or SerpAPI—using only the most appropriate source based on the query.

## Input Details
The workflow is triggered manually or via an API call with a user query (e.g., 'can you get me 3 articles about the election').

## Process Summary
The workflow starts with a user query passed to the Research Agent. The agent uses an OpenAI language model to decide which tool—Wikipedia, Hacker News, or SerpAPI—to use for answering the query, following a priority order. It first attempts Wikipedia, then Hacker News if needed, and finally SerpAPI as a fallback. Only one tool is invoked per query based on relevance. The result from the selected tool is then returned as the output.

## Output Details
The workflow returns the research result (e.g., articles or information) retrieved from the chosen source as a structured response.

## Tags
AI Agent, Research, Wikipedia, Hacker News, SerpAPI, OpenAI, Information Retrieval
