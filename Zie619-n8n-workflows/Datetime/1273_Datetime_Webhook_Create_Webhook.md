# Workflow Analysis for AI-Generated Summary Block for WordPress Posts - with OpenAI, WordPress, Google Sheets & Slack

## Description
This workflow automatically adds an AI-generated summary block at the top of new or unsummarized WordPress posts. It uses OpenAI to create concise bullet-point summaries, updates the post in WordPress, logs the summary in Google Sheets, and sends a notification to a Slack channel.

## Input Details
The workflow can be triggered manually, via a scheduled interval, or by a webhook when a new WordPress post is published.

## Process Summary
The workflow first retrieves WordPress posts either manually, on a schedule, or via webhook. It loops through each post and checks if it already has an AI summary by querying a Google Sheet using the post ID. If not summarized, it fetches the full post content, converts HTML to Markdown, and uses a text classifier to double-check for existing summaries. If confirmed as unsummarized, it sends the content to OpenAI with a custom prompt to generate a formatted HTML summary block. The workflow then updates the WordPress post with the new summary, logs the post details in Google Sheets, and sends a notification to Slack.

## Output Details
The workflow updates the WordPress post with an AI-generated HTML summary block, adds a record to a Google Sheet with post metadata and the summary, and sends a formatted notification to a Slack channel.

## Tags
WordPress, OpenAI, AI Summary, automation, Google Sheets, Slack, content summarization, n8n, production-ready
