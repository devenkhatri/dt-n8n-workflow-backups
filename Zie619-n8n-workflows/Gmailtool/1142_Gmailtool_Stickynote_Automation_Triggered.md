# Workflow Analysis for DeepSeek v3.1

## Description
This workflow automatically creates and publishes SEO-optimized blog content when a Notion database entry is updated, then notifies via email and updates the original Notion record with the published article details.

## Input Details
The workflow is triggered by updates to a specific Notion database (ID: 1c33d655-0fd9-8057-ac1a-eabf12d12f6b), polling hourly for changes.

## Process Summary
When a Notion page is updated, the workflow captures the entry's name as the topic. It uses AI instructions to generate an SEO-optimized blog post of up to 20 lines. The post is published to WordPress as a draft, and an email containing the title and URL is sent via Gmail. The workflow then retrieves available Notion tools and uses one to update the original Notion database entry with the article title, content, URL, and a 'publish' status.

## Output Details
The workflow publishes a blog post to WordPress, sends a confirmation email with the article link, and updates the corresponding Notion database record with the published content and status.

## Tags
Notion, WordPress, Gmail, AI, SEO, automation, content publishing, n8n, production-ready
