# Workflow Analysis for Threads Post Automation to Notion

## Description
This workflow automatically fetches your recent Threads posts (including text and media), checks if they already exist in a Notion database, and creates a new page in Notion for any new posts—complete with embedded media and metadata.

## Input Details
The workflow is triggered on a schedule and receives no external input; it uses stored credentials and environment variables to authenticate with Threads API and Notion.

## Process Summary
The workflow starts by refreshing a long-lived Threads API access token. It then fetches recent Threads posts from the last day, filters them by supported media types, and extracts key details like ID, permalink, and timestamp. Using a Notion database, it checks whether each post ID already exists to avoid duplicates. For new posts, it formats the content—including text and media URLs—into Notion-compatible blocks and creates a new database page with the post data. Finally, it uploads media by patching the Notion page with embed blocks.

## Output Details
The workflow creates new pages in a specified Notion database for each new Threads post, including post text, timestamp, permalink, username, and embedded media (images, videos, etc.).

## Tags
Threads, Notion, social media automation, API integration, scheduled workflow, content archiving, n8n
