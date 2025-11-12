# Workflow Analysis for Publish Videos & Images - Blotato

## Description
This workflow automates the publishing of videos and images to multiple social media platforms (Instagram, Facebook, YouTube, TikTok, Pinterest, LinkedIn, Twitter, Threads, and Bluesky) using Blotato as the publishing service. It pulls content from Airtable, uploads media to Blotato, generates a viral YouTube title using AI, and posts to each platform with appropriate formatting.

## Input Details
The workflow is triggered manually or via a test button and receives content data (including video URL, image URL, scripts, and platform-specific text) from an Airtable record identified by a hardcoded record ID.

## Process Summary
The workflow starts by fetching content details from a specific Airtable record. It then uploads the video and image assets to Blotato for hosting. Using OpenAI, it generates a viral YouTube title if needed. The workflow prepares platform-specific post data, including account IDs and media URLs. Finally, it sends parallel HTTP requests to Blotato to publish the content to nine different social media platforms with customized text and settings for each.

## Output Details
The workflow publishes content to Instagram, Facebook, YouTube, TikTok, Pinterest, LinkedIn, Twitter, Threads, and Bluesky via Blotato, and updates the original Airtable record's status to 'Completed' or 'In progress'.

## Tags
social media automation, multi-platform publishing, Blotato integration, Airtable integration, video publishing, image publishing, AI title generation, n8n workflow
