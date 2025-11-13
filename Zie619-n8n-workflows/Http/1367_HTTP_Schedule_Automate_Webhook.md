# Workflow Analysis for Auto-Post to Social Media Networks

## Description
This workflow automates the publishing of video content across nine social media platforms using the Blotato API, eliminating the need for manual posting.

## Input Details
The workflow is triggered daily at 10 PM and retrieves video details including URL, title, and description from a Google Sheet.

## Process Summary
First, the workflow is activated by a daily schedule. It then fetches video information and its row number from a specified Google Sheet. Next, it defines various social media account IDs. The video is then uploaded to Blotato via an HTTP request. Subsequently, the workflow sends out HTTP requests to Blotato's API to publish the video and its description to Instagram, YouTube, TikTok, Facebook, Threads, Twitter, LinkedIn, Bluesky, and Pinterest. Finally, it updates the Google Sheet, marking the video's status as 'DONE'.

## Output Details
The workflow publishes videos to Instagram, YouTube, TikTok, Facebook, Threads, Twitter, LinkedIn, Bluesky, and Pinterest, and updates the processing status in the source Google Sheet.

## Tags
automation, n8n, production-ready, excellent, optimized, social media, auto-post, video, blotato, google sheets
