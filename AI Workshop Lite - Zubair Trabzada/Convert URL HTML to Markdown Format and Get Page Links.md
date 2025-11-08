# Workflow Analysis for Convert URL HTML to Markdown and Get Page Links

## Description
This workflow converts web page content from HTML to markdown format, extracts all links from each page, and handles API rate limiting. It is designed for processing web content for LLM analysis, providing clean, formatted text without HTML markup, and extracting both content and links from web pages in batches.

## Input Details
The workflow is manually triggered or receives a list of URLs from a connected user-defined data source, where each URL is provided in a column named `Page`.

## Process Summary
1. The workflow begins with a manual trigger or by retrieving a list of URLs from a user-defined data source. 2. It then splits these URLs individually and processes them in batches of 40, further dividing each into sub-batches of 10. 3. For each URL, it sends an HTTP POST request to the Firecrawl.dev API to scrape the page, converting its HTML content into markdown and extracting all internal and external links. 4. A 45-second wait period is implemented between processing batches to adhere to API rate limits. 5. Finally, it extracts the page's title, description, markdown content, and links from the Firecrawl API response.

## Output Details
The extracted title, description, markdown content, and links for each processed URL are outputted to a user-defined data source, such as Airtable.
