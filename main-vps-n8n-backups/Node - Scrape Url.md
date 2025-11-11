# Workflow Analysis for Node - Scrape Url

## Description
This workflow scrapes a given web page URL and extracts the main article content in markdown format along with high-quality image URLs that are part of the main content.

## Input Details
The workflow is triggered manually or via another workflow and receives a single input: the URL of the web page to scrape.

## Process Summary
The workflow starts by receiving a URL as input. It then sends a POST request to the Firecrawl API with specific instructions to extract only the main content of the page in markdown format and to identify relevant images (at least 600px wide) within that main content. The API is configured to exclude non-essential elements like headers, footers, and ads. The response includes the cleaned main content and a list of qualifying image URLs. The workflow handles errors by retrying up to three times with a 5-second delay between attempts.

## Output Details
The workflow outputs the extracted main content in markdown and an array of relevant image URLs from the scraped web page, which can be used in downstream processes or returned as an API response.

## Tags
web scraping, content extraction, Firecrawl API, markdown, image extraction
