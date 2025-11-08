# Workflow Analysis for Website Content and Image Scraper

## Description
This workflow scrapes a given URL to extract the main content of a webpage in markdown format and identifies large, relevant images present within that main content using the Firecrawl API.

## Input Details
The workflow is triggered manually or by another workflow, receiving a URL as input.

## Process Summary
The workflow initiates by accepting a URL. It then sends an HTTP POST request to the Firecrawl API to scrape the provided URL. The scraping process is configured to extract the main content in various formats, exclude specific HTML elements, and focus solely on the primary content. It utilizes a detailed prompt and a JSON schema to accurately extract the verbatim main text content as markdown and an array of image URLs, ensuring extracted images are at least 600 pixels wide and integral to the main content.

## Output Details
The workflow produces a structured JSON output containing the extracted main content in markdown format and a list of relevant image URLs from the webpage.
