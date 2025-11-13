# Workflow Analysis for Social Media AI Agent - Telegram

## Description
Automated workflow: Social Media AI Agent - Telegram. This workflow integrates 15 different services: filter, markdown, httpRequest, stickyNote, airtable. It contains 32 nodes and follows best practices for error handling and security.

## Input Details
This workflow is triggered every 6 hours by a scheduler and starts by fetching content from a specified URL.

## Process Summary
First, the workflow crawls Hacker News to extract metadata for GitHub posts. It then checks an Airtable database to filter out any posts that have already been shared on social media. For new posts, the workflow visits the GitHub page, converts its content to Markdown, and uses an AI to generate engaging Twitter and LinkedIn posts. Finally, it stores these generated posts in Airtable, sends a notification via Telegram, and after a short wait, publishes the content to both Twitter and LinkedIn.

## Output Details
The workflow updates an Airtable database with post information and publishing status, sends notifications via Telegram, and publishes content to Twitter and LinkedIn.

## Tags
automation,n8n,production-ready,excellent,optimized,social media,ai,telegram,twitter,linkedin,airtable,hacker news,content creation
