# Workflow Analysis for Content - Short Form News Script Generator

## Description
This workflow automatically curates the top AI news stories from markdown files and Twitter posts for a given day, then generates engaging short-form video scripts optimized for platforms like TikTok and Instagram Reels. It identifies the most viral-worthy content based on impact, practicality, and audience engagement potential, then creates compelling hooks and full scripts for social media content creation.

## Input Details
The workflow is triggered either on a schedule (daily at 7 PM) or manually, and receives a date parameter to determine which day's content to process from an S3 bucket.

## Process Summary
The workflow first retrieves markdown files and Twitter posts from an S3 bucket for the specified date, filtering out newsletters and non-markdown content. It then aggregates and formats this content, sending it to an AI model that selects 3-5 top stories based on viral potential using specific curation criteria. For each selected story, the workflow scrapes the original source URLs for additional context, then uses another AI model to generate two complete short-form video scripts (140-160 words each) with compelling hooks. Finally, it posts the selected stories and generated scripts to a designated Slack channel for review and use.

## Output Details
The workflow outputs the curated top stories with summaries, hook angles, and source URLs, along with two complete video scripts for each story, all posted to a specific Slack channel for the content team to review and use.

## Tags
content creation, AI news, short-form video, social media, script generation, news curation, automation, TikTok, Instagram Reels, Slack integration
