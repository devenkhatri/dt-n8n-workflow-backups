# Workflow Analysis for API Calls in n8n

## Description
This workflow demonstrates various ways to make external API calls in n8n, including using native nodes, raw HTTP requests, and AI-powered agents that can perform web searches and fetch real-time data.

## Input Details
The workflow is triggered by a chat message sent to a webhook endpoint, and also includes a hardcoded query for demonstration purposes.

## Process Summary
The workflow starts when a chat message is received, which activates an AI agent powered by GPT-4.1-mini. The agent can use a web search tool (Perplexity API) to fetch information. Separately, the workflow shows two approaches to get weather data for Chicago: using the native OpenWeatherMap node and a raw HTTP request to the same API. Another branch demonstrates making a search request to Tavily by first setting a sample query ('pineapples on pizza') and then sending it via HTTP POST.

## Output Details
The workflow doesn’t send output to external systems in this version but is designed to showcase API integration patterns; results from API calls would typically be used by the AI agent or passed to downstream nodes in a real-world scenario.

## Tags
API, HTTP Request, AI Agent, OpenWeatherMap, Perplexity, Tavily, Webhook, Chat Trigger, n8n
