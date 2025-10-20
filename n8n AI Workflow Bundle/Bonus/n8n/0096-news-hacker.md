# Workflow Analysis for News Hacker Workflow

## Description
This workflow summarizes news articles from Hacker News and posts the summaries to a Discord channel.

## Input Details
This workflow is triggered every 30 minutes by a schedule trigger.

## Process Summary
The workflow first fetches the top 10 articles from Hacker News. It then iterates through each article, fetching its content. For each article, it checks if the content is available; if so, it constructs a prompt to summarize the article and uses OpenAI to generate a summary. Finally, it formats the summary with the article title and URL.

## Output Details
The workflow posts the summarized news articles to a specified Discord channel.
