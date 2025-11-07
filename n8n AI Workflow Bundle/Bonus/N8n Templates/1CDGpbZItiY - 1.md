# Workflow Analysis for Advanced Multi-Purpose Web Scraper

## Description
This workflow demonstrates various web scraping techniques using the Crawl4AI service, including extracting sitemap URLs, scraping full page content into Markdown, extracting structured data using LLMs, and performing large-scale CSS-based data extraction. It also includes an AI agent for interactive assistance.

## Input Details
The workflow is primarily triggered manually but also contains a chat trigger for an AI expert, receiving user input or a test workflow signal.

## Process Summary
1. Upon manual activation, the workflow extracts a list of URLs from a sitemap XML using an AI agent (Google Gemini) and a structured output parser. 2. It then sends a request to a Crawl4AI endpoint to crawl these URLs and retrieve their content as Markdown, continuously polling for results. 3. Separately, it initiates an LLM-based crawl using OpenAI GPT-4o-mini to extract structured pricing information from the Gemini API documentation page, also polling for completion. 4. Concurrently, it performs a large-scale CSS-based extraction to scrape product details, including ratings, from multiple pages of an e-commerce sandbox, polling until all data is retrieved. 5. Finally, the CSS-extracted product data is processed to calculate star counts and is then converted into a CSV file. The workflow also includes an AI agent (Crawl4AI Expert) that can respond to chat messages using Google Gemini and has access to extensive Crawl4AI documentation.

## Output Details
The workflow produces markdown content from various URLs, structured JSON data containing AI model pricing information, and a CSV file containing structured product details.
