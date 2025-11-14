# Workflow Analysis for YouTube Videos with AI Summaries on Discord

## Description
This workflow automatically detects new YouTube videos from a specified channel, retrieves their English captions, generates a three-bullet-point summary using AI, and then posts this information along with a link to the video on a Discord channel.

## Input Details
The workflow is triggered every minute by new video entries in a YouTube channel's RSS feed.

## Process Summary
1. The workflow starts by monitoring a YouTube channel's RSS feed for new video uploads.
2. Upon detecting a new video, it retrieves available caption data for that video and specifically identifies the English captions.
3. It then downloads the content of these English captions.
4. The downloaded caption file is converted to plain text.
5. This text transcript is then sent to ChatGPT, which generates a concise three-bullet-point summary of the video.

## Output Details
The workflow posts a formatted message containing the new YouTube video's title, a link to the video, and an AI-generated three-bullet-point summary to a designated Discord channel.

## Tags
YouTube, AI, Discord, Video Summary, Automation, RSS, Caption, ChatGPT, n8n
