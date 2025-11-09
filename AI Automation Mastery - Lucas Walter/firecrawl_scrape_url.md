# Workflow Analysis for Node - Scrape Url

## Description
This workflow scrapes a given web URL to extract the main content and relevant high-resolution images using the Firecrawl API. It focuses only on the core article or newsletter body, excluding ads, headers, footers, and non-essential elements.

## Input Details
The workflow is triggered manually or by another workflow and receives a single input: the URL to be scraped.

## Process Summary
The workflow starts by receiving a URL input. It then sends a POST request to the Firecrawl API with instructions to scrape the page, extract only the main content in markdown format, and identify image URLs within that content that are at least 600px wide. The API is instructed to exclude navigation elements, banners, and promotional content. The response includes the clean main content and an array of qualified image URLs.

## Output Details
The workflow outputs structured data containing the main content of the page in markdown format and an array of relevant, high-resolution image URLs extracted from the main content.

## Tags
web scraping, content extraction, Firecrawl, markdown, images, main content, API integration
