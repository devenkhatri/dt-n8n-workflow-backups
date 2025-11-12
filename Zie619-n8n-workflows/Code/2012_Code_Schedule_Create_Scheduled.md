# Workflow Analysis for News Extraction

## Description
This workflow automatically scrapes news articles from a website that doesn't provide an RSS feed, filters the latest posts from the past 70 days, generates a short summary and extracts technical keywords for each article using OpenAI's GPT-4, and stores the structured results (title, date, link, summary, and keywords) in a NocoDB database.

## Input Details
The workflow is triggered weekly by a cron schedule and starts by fetching the HTML content of a news webpage specified by the WEBHOOK_URL environment variable.

## Process Summary
First, the workflow retrieves the main news page and extracts publication dates and individual article links using CSS selectors. It converts these extracted arrays into individual items, merges date and link data, and filters only posts from the last 70 days. For each recent article, it fetches the full HTML, extracts the title and content, then sends the content to OpenAI to generate a summary and identify three technical keywords. Finally, it merges all data (title, date, link, summary, keywords) and saves each article's structured information to a NocoDB database.

## Output Details
The workflow outputs structured news data (title, date, link, summary, and keywords) to a NocoDB database table for further use or analysis.

## Tags
news scraping, web scraping, OpenAI, GPT-4, NocoDB, automation, content summarization, keyword extraction, scheduled workflow, HTML parsing
