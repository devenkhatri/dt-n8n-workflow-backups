# Workflow Analysis for Convert URL HTML to Markdown and Get Page Links

## Description
This workflow fetches web pages from a list of URLs and converts their HTML content into clean, AI-friendly markdown while also extracting all links from each page. It handles rate limits and processes URLs in manageable batches to avoid memory or API issues.

## Input Details
The workflow is triggered manually and receives a list of URLs, either from an example array in the workflow or from a connected external data source with a column named 'Page'.

## Process Summary
The workflow starts by accepting a list of URLs and splitting them into individual items. It limits processing to 40 URLs at a time to manage memory, then further splits them into batches of 10 to respect the Firecrawl API rate limit of 10 requests per minute. Each URL is sent to the Firecrawl.dev API to retrieve its markdown content and links. The response is reformatted to extract title, description, content, and links into separate fields.

## Output Details
The processed data—title, description, markdown content, and links for each URL—is sent to the user's connected output data source, such as a database or Airtable.

## Tags
web scraping, markdown conversion, firecrawl, API integration, batch processing, rate limiting, URL processing, data extraction
