# Workflow Analysis for News Extraction

## Description
This workflow automatically scrapes news articles from a website that doesn't provide an RSS feed, filters the latest posts from the past 70 days, generates a short summary and extracts technical keywords for each article using AI, and stores the structured data in a NocoDB database.

## Input Details
The workflow is triggered weekly by a schedule trigger and starts by fetching HTML content from a predefined news website URL stored in an environment variable.

## Process Summary
First, the workflow retrieves the main news page and extracts individual post links and their publication dates using CSS selectors. It then filters posts from the last 70 days. For each recent post, it fetches the full HTML content, extracts the title and article text, and sends this content to OpenAI to generate a concise summary and three technical keywords. The summary and keywords are cleaned up and merged with the post's title, date, and link. Finally, this enriched data is stored in a NocoDB database.

## Output Details
The workflow outputs structured news data—title, date, link, summary, and keywords—for each recent article into a NocoDB database table.

## Tags
news scraping, web scraping, OpenAI, GPT-4, NocoDB, automation, content summarization, keyword extraction, scheduled workflow, HTML parsing
