# Workflow Analysis for Get a Web Page

## Description
This workflow is designed to crawl a given web page and extract its content, specifically in markdown format. It is optimized for production use and can be easily integrated with AI agents or other workspaces.

## Input Details
The workflow is triggered by an external request (e.g., a webhook) that provides the URL of the web page to be crawled.

## Process Summary
1. The workflow is initiated by a trigger that receives a URL. 2. It then uses the FireCrawl service to crawl the provided URL and retrieve its content, formatted as markdown. 3. Finally, it extracts the markdown content from the FireCrawl response and assigns it to a field named "response".

## Output Details
The workflow outputs the markdown-formatted content of the crawled web page, available to the requesting system or agent.

## Tags
automation, n8n, production-ready, excellent, optimized
