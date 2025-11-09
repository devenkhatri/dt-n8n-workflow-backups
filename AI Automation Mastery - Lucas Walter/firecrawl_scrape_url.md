# Workflow Analysis for Node - Scrape Url

## Description
This workflow scrapes a given web page URL and extracts the main content along with relevant high-resolution image URLs using an AI-powered scraping service.

## Input Details
The workflow is triggered with a single input: a URL to be scraped.

## Process Summary
The workflow starts by receiving a URL as input. It then sends a POST request to the Firecrawl API with specific instructions to extract only the main content of the page in markdown format and to identify image URLs within that main content that are at least 600px wide. The request excludes non-essential page elements like headers, footers, and ads. The AI processes the page based on the provided prompt and schema to return structured data containing the content and relevant image URLs.

## Output Details
The workflow outputs structured JSON data containing the main content in markdown and an array of relevant image URLs from the scraped web page.

## Tags
scraping, web content extraction, AI parsing, markdown, image extraction
