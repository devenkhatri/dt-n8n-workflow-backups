# Workflow Analysis for The Recap AI - Repurpose YouTube Video To Socials

## Description
This workflow automatically transforms a YouTube video into engaging promotional content for Twitter and LinkedIn. It extracts the video's transcript, then uses AI to generate multiple post options for each platform based on proven viral examples, helping users quickly create high-performing social media content that drives engagement and followers.

## Input Details
The workflow is triggered by a form submission containing a YouTube video URL.

## Process Summary
The workflow starts by scraping the YouTube video's transcript and metadata using Apify. It then prepares sets of example Twitter and LinkedIn posts to guide content generation. Using a powerful AI model (Claude Sonnet), it creates three distinct Twitter tweets and three LinkedIn posts based on the video content and the example structures. Finally, all generated content options are sent to a Slack channel for review, organized in threaded messages linked to the original video.

## Output Details
The workflow produces three Twitter tweet options and three LinkedIn post options, which are posted as threaded messages in a specified Slack channel for user review and selection.

## Tags
youtube, social media, content repurposing, twitter, linkedin, ai content, automation, slack, transcript, viral content
