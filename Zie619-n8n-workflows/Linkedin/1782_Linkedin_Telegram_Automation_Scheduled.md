# Workflow Analysis for Social Media AI Agent - Telegram

## Description
This automated workflow integrates multiple services to curate and share trending GitHub discussions from Hacker News to Twitter and LinkedIn, leveraging AI to generate engaging posts.

## Input Details
This workflow is triggered every 6 hours by a schedule, initiating the content curation process.

## Process Summary
First, the workflow crawls Hacker News, extracts GitHub links, and fetches their metadata. It then checks an Airtable database to avoid posting duplicate content. For new items, it visits the GitHub page, converts the content to Markdown, and uses an AI model to generate tailored posts for Twitter and LinkedIn. Finally, it stores the generated content in Airtable, sends a Telegram notification to the owner, waits for 5 minutes, and then publishes the posts to Twitter and LinkedIn, updating their status in Airtable.

## Output Details
The workflow publishes generated social media posts to Twitter and LinkedIn, updates records in an Airtable database, and sends a Telegram notification.

## Tags
automation,n8n,production-ready,excellent,optimized
