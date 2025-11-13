# Workflow Analysis for Stickynote Workflow

## Description
This workflow fetches and processes web page content based on a query string provided by an AI agent. It supports two modes — full or simplified — and converts the cleaned HTML into Markdown while enforcing a maximum content length to optimize token usage.

## Input Details
The workflow is triggered by another workflow or an AI agent and receives a query string containing URL and processing method parameters.

## Process Summary
First, the query string is parsed into a JSON object and a maximum content length is set. An HTTP request fetches the webpage, and if an error occurs, a descriptive message is returned. If successful, the HTML body is extracted and unnecessary tags (like scripts, styles, and media) are removed. If the 'simplified' method is specified, URLs and image sources are replaced with placeholders. Finally, the cleaned HTML is converted to Markdown, and the output is truncated or replaced with an error if it exceeds the allowed length.

## Output Details
The workflow returns the processed page content as Markdown or an error message, which is then sent back to the calling AI agent or workflow.

## Tags
web scraping, HTML processing, markdown conversion, AI agent, error handling, content filtering, automation
