# Workflow Analysis for Get a Web Page

## Description
This workflow fetches the content of a web page by sending a URL to a crawling service and returns the page content formatted as Markdown.

## Input Details
The workflow is triggered manually or by another workflow and receives a JSON input containing a 'url' field specifying the web page to crawl.

## Process Summary
The workflow starts with an Execute Workflow Trigger that accepts a URL input. It then sends a POST request to the FireCrawl API with the provided URL, requesting the page content in Markdown format. The API response is processed to extract the Markdown content from the 'data.markdown' field. Finally, the extracted content is assigned to a new field called 'response' for output.

## Output Details
The workflow outputs a JSON object containing the crawled web page content as a Markdown string in the 'response' field.

## Tags
web scraping, markdown, automation, n8n, production-ready, API integration, content extraction
