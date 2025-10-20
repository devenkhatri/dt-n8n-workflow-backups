# Workflow Analysis for TechRadar AI Agent for Article Scraping and Summarization

## Description
This workflow automates the process of extracting articles from TechRadar, summarizing them using AI, and then storing the summaries in a Google Sheet and a local file for future reference.

## Input Details
The workflow is manually triggered and uses a predefined TechRadar URL for article extraction.

## Process Summary
First, the workflow identifies all articles on the TechRadar webpage using a CSS selector. Then, it iterates through each article, extracts the content, and generates a concise summary using the OpenAI API. The workflow checks if a summary is already available in the Google Sheet; if not, it processes the article. Finally, both raw and summarized content are saved into a new Google Sheet row and also appended to a local JSON file.

## Output Details
The workflow outputs article summaries and raw content to a Google Sheet and a local JSON file.
