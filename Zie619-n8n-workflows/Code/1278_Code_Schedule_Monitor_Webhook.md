# Workflow Analysis for AI-Powered Information Monitoring with OpenAI, Google Sheets, Jina AI and Slack

## Description
This workflow automatically monitors RSS feeds for new articles relevant to AI and data science topics, summarizes the relevant ones using OpenAI, and posts formatted summaries to a Slack channel—all while avoiding duplicate processing by tracking articles in Google Sheets.

## Input Details
The workflow is triggered on a schedule (every 15 minutes by default) and receives RSS feed URLs and article data from a Google Sheet, along with previously processed article records from another sheet in the same document.

## Process Summary
The workflow starts by fetching a list of RSS feed URLs and previously processed articles from Google Sheets. It then reads new articles from the RSS feeds and filters out any already processed. Each new article is sent to OpenAI to classify its relevance to AI/data topics. Non-relevant articles are logged in Google Sheets. Relevant articles are fetched in full using Jina AI, summarized by OpenAI in Slack-compatible Markdown format, posted to a Slack channel, and recorded in Google Sheets with metadata like URL, summary, and publish date.

## Output Details
The workflow posts AI-generated, Slack-formatted article summaries to a designated Slack channel and logs all processed articles (both relevant and not) in a Google Sheet for tracking and deduplication.

## Tags
AI monitoring, RSS automation, OpenAI, Slack integration, Google Sheets, Jina AI, content summarization, topic filtering, workflow automation, n8n
