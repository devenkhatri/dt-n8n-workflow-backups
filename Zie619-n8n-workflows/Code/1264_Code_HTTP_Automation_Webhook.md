# Workflow Analysis for Complete Youtube

## Description
This workflow helps YouTube creators discover trending content in their niche by analyzing recent high-performing videos and providing data-driven insights on current trends, including view counts, likes, comments, tags, and channel information.

## Input Details
The workflow is triggered manually or via a chat message webhook and receives a user-provided content niche or query as input.

## Process Summary
The workflow starts by receiving a niche or query from the user. It then searches YouTube for the top 3 most relevant videos from the last 2 days using that niche. For each video, it fetches detailed metadata including statistics and descriptions, filters out videos shorter than 3 minutes 30 seconds, and cleans the data by removing emojis and URLs. The processed video data is stored in memory and aggregated. Finally, the AI agent analyzes the collected data to identify content patterns and trends, then delivers a summary with insights and links to the relevant videos and channels.

## Output Details
The workflow returns a summarized trend analysis with embedded video and channel links, formatted as a response from an AI agent to guide content creators.

## Tags
youtube, trending analysis, content creation, AI agent, video analytics, automation, n8n, production-ready
