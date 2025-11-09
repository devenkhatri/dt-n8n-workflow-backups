# Workflow Analysis for The Recap AI - Repurpose YouTube Video To Socials

## Description
This workflow automatically transforms a YouTube video into engaging social media content tailored for Twitter and LinkedIn. It extracts the video transcript, analyzes it, and uses AI to generate multiple post options based on proven viral templates for each platform.

## Input Details
The workflow is triggered by a form submission containing a YouTube video URL.

## Process Summary
The workflow starts by scraping the YouTube video's transcript and metadata using an Apify actor. It then prepares sets of example posts for both Twitter and LinkedIn. Using these examples as templates, it constructs detailed prompts for an AI language model (Claude Sonnet 4) to generate three distinct, high-potential post options for each platform. The AI's output is parsed into a structured format and sent to a Slack channel for review, with each option posted as a reply in a thread under a main message that includes the original YouTube video link.

## Output Details
The workflow produces three Twitter post options and three LinkedIn post options, which are posted as threaded messages in a specified Slack channel for user review and selection.

## Tags
youtube, social media, repurpose, twitter, LinkedIn, AI, content creation, automation, n8n, Claude AI
