# Workflow Analysis for AI-Generated Summary Block for WordPress Posts - with OpenAI, WordPress, Google Sheets & Slack

## Description
This workflow automatically adds an AI-generated summary at the top of new or existing WordPress posts. It uses OpenAI to create concise summaries, checks if a post has already been summarized using Google Sheets, updates the post with the new summary while preserving the original excerpt, logs the action in Google Sheets, and sends a notification to a Slack channel.

## Input Details
The workflow can be triggered manually, via a scheduled interval to fetch recent WordPress posts, or by a webhook that receives a new post ID when a post is published.

## Process Summary
The workflow first retrieves WordPress posts either manually, on a schedule, or via webhook. It loops through each post and checks a Google Sheet to see if the post has already been summarized. If not, it fetches the full post content, converts HTML to Markdown, and sends it to OpenAI with instructions to generate a formatted HTML summary block. After receiving the summary, it updates the WordPress post by prepending the summary, logs the post details in Google Sheets, and notifies a Slack channel.

## Output Details
The workflow updates WordPress posts with AI-generated HTML summary blocks, records summarized posts in a Google Sheet, and sends a formatted notification to a Slack channel.

## Tags
WordPress, OpenAI, AI Summary, Google Sheets, Slack, automation, content summarization, n8n, production-ready
