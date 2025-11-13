# Workflow Analysis for Search news using Perplexity AI and post to X (Twitter)

## Description
This workflow automates the process of finding the latest news in artificial intelligence using Perplexity AI and then publishing a concise summary of a single article, along with its link, to X (Twitter).

## Input Details
The workflow is triggered automatically every 21 hours by a schedule trigger, requiring no manual input beyond its initial setup.

## Process Summary
The workflow is initiated every 21 hours by a schedule trigger. It defines a search query for "What's the latest news in artificial intelligence?". An API key for Perplexity AI is configured. It sends an HTTP request to Perplexity AI to search for news based on the query, with instructions to generate a short, engaging headline and a direct article link, formatted for X (Twitter). Finally, the generated news summary and link are posted to a configured X (Twitter) account.

## Output Details
The workflow posts a summarized artificial intelligence news headline and its direct link to X (Twitter).

## Tags
automation, n8n, production-ready, excellent, optimized
