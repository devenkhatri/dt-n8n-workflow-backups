# Workflow Analysis for Content - Short Form News Script Generator

## Description
This workflow automatically generates viral short-form video scripts based on the latest AI news content. It retrieves markdown articles and tweets from a specific date, filters out newsletters, selects the top 3-5 most engaging stories using AI, and then creates two polished video scripts with compelling hooks for each story.

## Input Details
The workflow is triggered either on a daily schedule at 7 PM or manually with an optional date parameter, and it pulls content from S3 buckets containing markdown files and tweet data for that date.

## Process Summary
First, the workflow fetches markdown and tweet content from an S3 bucket for a given date, filtering out newsletter content and non-markdown files. It then aggregates and formats this content before using a large language model (Claude) to select the top 3-5 stories based on virality potential. For each selected story, the workflow scrapes the original source URLs, then uses another LLM prompt to generate two complete 50-60 second video scripts with multiple hook options. Finally, it posts the selected stories and their corresponding scripts to a designated Slack channel with threading for easy review.

## Output Details
The workflow outputs curated AI news stories with multiple hook angles and two complete short-form video scripts per story, all posted to a specific Slack channel with source links and scraped content for context.

## Tags
AI, content creation, short-form video, script generation, news curation, social media, Slack integration, Claude AI, viral content
