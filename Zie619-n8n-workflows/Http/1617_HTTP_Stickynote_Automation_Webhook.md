# Workflow Analysis for Tavily Search & Extract - Template

## Description
This workflow demonstrates how to use the Tavily API for intelligent web searching and content extraction, followed by AI-powered summarization of the extracted web pages.

## Input Details
The workflow is triggered manually or by providing a search topic via a chat window, and it utilizes a predefined Tavily API key.

## Process Summary
First, the workflow sets the Tavily API key and receives a search query. It then performs a Tavily search based on the query, including images and descriptions. The search results are filtered to retain only highly relevant items (score > 0.80). Next, it extracts the raw content from the URL of the top search result using the Tavily Extract API. Finally, an OpenAI Chat Model is used to summarize the extracted web page content into Markdown format.

## Output Details
The workflow produces a Markdown-formatted summary of the web page content from the most relevant search result.

## Tags
automation, n8n, Tavily, search, web scraping, AI, summarization, OpenAI, content extraction, production-ready
