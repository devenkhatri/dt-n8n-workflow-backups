# Workflow Analysis for News Article Summarization and Keyword Extraction for NocoDB

## Description
This workflow scrapes news articles from a specified website, extracts recent posts, generates a summary and relevant technical keywords for each, and then stores this processed information into a NocoDB database.

## Input Details
The workflow is automatically triggered once a week by a schedule, initiating the web scraping process.

## Process Summary
First, the workflow fetches the main news page and extracts links and publication dates for all articles. It then filters these articles to only process those published within the last seven days. For each recent article, it retrieves the full content from its unique URL, extracts the title and body, and subsequently uses OpenAI to generate a concise summary and identify three key technical keywords. All this information is then consolidated.

## Output Details
The workflow produces structured data containing the news article's title, date, link, AI-generated summary, and keywords, which is then stored in a NocoDB database.
