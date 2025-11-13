# Workflow Analysis for Extract And Decode Google News RSS URLs to Clean Article Links

## Description
This workflow automates the process of extracting and decoding Google News RSS feed URLs to obtain clean, direct article links. It's designed for production use with error handling and security considerations.

## Input Details
The workflow is triggered manually and reads news articles from a specified Google News RSS feed URL, typically receiving RSS feed items.

## Process Summary
The workflow starts by reading items from a Google News RSS feed and limits the number of items processed. It then makes an HTTP request to retrieve the HTML content of each news item. From this HTML, it extracts necessary decoding keys, specifically a signature and timestamp. Using these keys and the article's unique ID, it prepares a request payload for a specific Google decoding service. An HTTP POST request is then sent to this service to decode the original Google News URL, and the response is parsed to extract the clean article link. Finally, all the resulting clean URLs are aggregated.

## Output Details
The workflow produces a collection of clean, direct article links from the Google News RSS feed, aggregated into a single object within the workflow.

## Tags
automation, n8n, production-ready, excellent, optimized
