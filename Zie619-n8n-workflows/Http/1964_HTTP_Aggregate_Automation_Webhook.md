# Workflow Analysis for Google Maps FULL

## Description
This is an AI-powered lead generation workflow designed to extract comprehensive business data from Google Maps and associated websites. It leverages AI to process user requests, orchestrates web scraping, and enriches data with fallback internet searches. The workflow is optimized for production use, includes robust error handling, and stores collected information in a structured manner.

## Input Details
The workflow is triggered by user messages or structured requests containing search parameters such as business type, city, state/county, and country code for lead generation.

## Process Summary
1. A user's message is processed by an AI agent and a GPT-4o model to identify business lead search parameters. 2. The "Tool - Scrape Google Maps Business Data" subworkflow then extracts business listings (name, address, phone, website) from Google Maps via Apify based on these parameters. 3. The extracted Google Maps data is saved to Google Sheets. 4. Concurrently, the "Tool - Crawl Business Website" subworkflow crawls the websites of the identified businesses using Apify to gather detailed content. 5. If initial scraping is incomplete, a fallback Google Search tool is used to enrich the data, and the crawled website content is also saved to Google Sheets.

## Output Details
The workflow produces organized business lead data (including names, addresses, phone numbers, and websites) and detailed website content, which are both stored in Google Sheets.

## Tags
automation, n8n, production-ready, excellent, optimized, lead generation, google maps, web scraping, AI, data extraction, google sheets
