# Workflow Analysis for Agent with custom HTTP Request

## Description
This n8n workflow functions as an AI agent with a custom HTTP request tool. It is designed for production use, featuring robust error handling, security measures, and comprehensive documentation.

## Input Details
This workflow is triggered by an AI agent calling a custom HTTP Request tool, which receives a query string containing a URL and a method (full or simplified) to fetch web page content.

## Process Summary
First, the workflow parses the incoming query string to extract the URL and method, setting a maximum page content limit. It then performs an HTTP request to the specified URL. If an error occurs during the request, an error message is generated. Otherwise, the HTML body is extracted, cleaned by removing scripts, styles, and other non-essential tags, and optionally simplified by removing links and image URLs. The cleaned HTML is then converted to Markdown format. Finally, the processed content is checked against a maximum length limit.

## Output Details
The workflow outputs the processed web page content in Markdown format or an error message if the HTTP request fails or the content exceeds the defined length limit, which is then consumed by the calling AI agent.

## Tags
automation, n8n, production-ready, excellent, optimized
