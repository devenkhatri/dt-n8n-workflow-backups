# Workflow Analysis for Content - Short Form News Script Generator

## Description
This workflow automatically curates the top AI-related news stories from markdown files and tweets for a given day, selects the most viral-worthy ones, and generates ready-to-use short-form video scripts with compelling hooks for social media platforms like TikTok and Instagram.

## Input Details
The workflow is triggered on a schedule (daily at 7 PM CT) or manually, and uses the current date (or a provided date) to fetch relevant markdown and tweet content from an S3 bucket.

## Process Summary
The workflow first retrieves markdown and tweet content from an S3 bucket for the specified date. It filters out newsletters and formats the content for analysis. A language model then analyzes all the content to select the top 3-5 most viral stories, generating multiple hook angles for each. The selected stories are posted to a Slack channel. For each story, the workflow scrapes the original source URLs for full context and uses another language model to generate two complete, polished short-form video scripts with strong hooks. These scripts are then shared as threaded replies in Slack under the original story post.

## Output Details
The workflow outputs curated story summaries and two professionally written short-form video scripts for each story, all posted to a designated Slack channel for the content team to review and use.

## Tags
content, ai, social media, script generation, news curation, short-form video, automation, slack
