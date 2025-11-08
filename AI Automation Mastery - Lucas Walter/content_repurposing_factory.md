# Workflow Analysis for AI-Powered YouTube Video to Social Media Repurposing

## Description
This workflow automates the process of transforming a YouTube video into multiple social media posts for Twitter and LinkedIn, leveraging AI to generate engaging content based on the video transcript and pre-defined examples.

## Input Details
The workflow is triggered by a form submission where the user provides a YouTube Video URL.

## Process Summary
First, the workflow scrapes the provided YouTube video to extract its transcript and other metadata. Then, it prepares detailed prompts for an AI model (Anthropic Claude Sonnet 4), including the YouTube transcript and a set of successful example posts for both Twitter and LinkedIn. The AI generates three distinct social media post options for each platform, adapting the structure and style from the examples. Finally, these generated post options are organized and sent to a designated Slack channel for review.

## Output Details
The workflow produces three unique Twitter post options and three unique LinkedIn post options, delivered to a Slack channel for content approval.
