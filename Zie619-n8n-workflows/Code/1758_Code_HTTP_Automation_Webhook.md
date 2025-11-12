# Workflow Analysis for Complete Youtube

## Description
This workflow helps YouTube creators discover trending content in their niche by analyzing recent high-performing videos and providing insights on patterns in titles, tags, and engagement metrics like views, likes, and comments.

## Input Details
The workflow is triggered manually or via a chat message and receives a user-defined content niche as input.

## Process Summary
The workflow starts by prompting the user to specify a niche if not already provided. It then uses the YouTube API to search for up to three recent (within the last 2 days) trending videos relevant to the niche. For each video, it fetches detailed statistics and metadata, filters out videos shorter than 3 minutes 30 seconds, and cleans the data by removing emojis, links, and extra whitespace. The processed video data is stored in global workflow memory, formatted with separators, and compiled into a single response string that highlights content trends across all retrieved videos.

## Output Details
The workflow produces a summarized insight report on current trends in the specified niche, including cleaned metadata and engagement metrics for relevant videos, which is stored in memory and can be accessed by an AI agent for user communication.

## Tags
youtube, trending videos, content analysis, ai agent, video insights, automation, n8n, production-ready
