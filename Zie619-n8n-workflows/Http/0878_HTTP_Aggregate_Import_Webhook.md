# Workflow Analysis for Apify YouTube MCP Server

## Description
This workflow enables a Model Context Protocol (MCP) server that allows AI agents or clients to search YouTube videos and retrieve their transcripts using the Apify scraping service. It also provides usage metrics for the Apify account.

## Input Details
The workflow is triggered by another workflow or an MCP client via a webhook, receiving an operation type (youtube_search, youtube_transcripts, or usage_metrics), an optional search query, and/or YouTube URLs.

## Process Summary
The workflow starts with an execution trigger that accepts operation type, query, and URLs. A switch node routes the execution based on the operation: 'youtube_search' sends a query to Apify to find videos; 'youtube_transcripts' fetches subtitles from provided YouTube URLs; and 'usage_metrics' retrieves current Apify account usage data. Each path processes and simplifies the API response, then aggregates results into a consistent output format.

## Output Details
The workflow returns structured data: either a list of YouTube search results, video transcripts, or current Apify usage metrics, which can be consumed by an MCP client or another workflow.

## Tags
youtube, apify, mcp server, transcripts, search, usage metrics, automation, n8n, ai agent
