# Workflow Analysis for YouTube Metadata Generator for SyncBricks

## Description
This workflow automatically generates SEO-optimized YouTube video titles, descriptions, tags, hashtags, and CTAs using AI, then updates the video on YouTube with the new metadata. It pulls relevant affiliate and promotional links from a Google Doc to include in the description.

## Input Details
The workflow is triggered by a form submission containing a YouTube video link, video transcript, and optional focus keywords.

## Process Summary
When the form is submitted, the workflow first extracts the YouTube video ID from the provided link. It then fetches relevant affiliate and promotional links from a predefined Google Doc. Using an AI model (configured as GPT-4o-mini), it generates a structured JSON output containing an optimized title, detailed description, tags, hashtags, and a call to action based on the transcript and keywords. The tags are formatted into a comma-separated string, and the YouTube video is updated with the new metadata. Finally, a confirmation message with the updated video title and link is displayed to the user.

## Output Details
The workflow updates the specified YouTube video with AI-generated metadata and shows a success form confirming the update with the new title and video link.

## Tags
youtube automation, ai content generation, seo optimization, metadata generator, gpt-4, google docs integration, n8n workflow, video optimization, affiliate marketing, syncbricks
