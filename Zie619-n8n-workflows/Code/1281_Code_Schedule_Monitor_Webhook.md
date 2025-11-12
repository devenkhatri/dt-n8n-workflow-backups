# Workflow Analysis for AI-Powered Information Monitoring with OpenAI, Google Sheets, Jina AI and Slack

## Description
This workflow automatically monitors RSS feeds for new articles related to AI and data science, uses AI to determine relevance, summarizes relevant articles, and posts clean, formatted summaries to a Slack channel—all while avoiding duplicate processing by tracking articles in Google Sheets.

## Input Details
The workflow is triggered on a schedule (every 15 minutes by default) and receives RSS feed URLs and previously processed article data from a Google Sheet.

## Process Summary
The workflow starts by fetching a list of RSS feed URLs and previously monitored articles from Google Sheets. It reads the RSS feeds, filters out any articles already processed, and checks each new article for relevance to AI/data topics using OpenAI. Relevant articles are fetched in full via Jina AI, summarized and formatted for Slack using GPT-4o-mini, then posted to a Slack channel. Both relevant and irrelevant articles are logged in Google Sheets to prevent reprocessing.

## Output Details
The workflow posts AI-generated, Slack-formatted summaries of relevant articles to a designated Slack channel and logs all processed article metadata (URL, relevance status, summary, publish date, etc.) in a Google Sheet.

## Tags
AI, automation, RSS, Slack, Google Sheets, OpenAI, Jina AI, content monitoring, summarization, n8n
