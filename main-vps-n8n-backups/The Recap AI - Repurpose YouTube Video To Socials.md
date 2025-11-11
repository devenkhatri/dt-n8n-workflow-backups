# Workflow Analysis for The Recap AI - Repurpose YouTube Video To Socials

## Description
This workflow automatically converts a YouTube video into engaging social media posts for Twitter/X and LinkedIn by analyzing the video transcript and generating multiple post options based on proven viral examples.

## Input Details
The workflow is triggered by a form submission containing a YouTube video URL.

## Process Summary
The workflow starts by scraping the YouTube video transcript and metadata using an Apify actor. It then prepares example tweets and LinkedIn posts as reference material. Using a powerful AI language model (Claude Sonnet 4), it generates three distinct Twitter post options and three LinkedIn post options based on the video content and the provided examples. The results are formatted into structured JSON responses and sent to a Slack channel as threaded messages for easy review and selection.

## Output Details
The workflow produces three Twitter post options and three LinkedIn post options, which are posted as threaded messages in a specified Slack channel for user review and selection.

## Tags
youtube, social media, content repurposing, AI writing, Twitter, LinkedIn, automation, n8n, Claude AI, Slack integration
