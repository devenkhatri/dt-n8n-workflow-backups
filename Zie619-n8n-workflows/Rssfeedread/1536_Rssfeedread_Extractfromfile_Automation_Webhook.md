# Workflow Analysis for YouTube Videos with AI Summaries on Discord

## Description
This workflow automatically detects new YouTube videos from a specified channel, retrieves their English captions, generates a three-bullet point summary using AI, and then posts this information, along with the video link, to a Discord channel.

## Input Details
The workflow is triggered by new videos appearing in a YouTube channel's RSS feed, receiving video metadata.

## Process Summary
1. It starts by monitoring a YouTube channel's RSS feed for new video uploads.
2. Upon detecting a new video, it retrieves available caption data for that video and specifically identifies the English captions.
3. The workflow then downloads the English caption file and extracts its textual content.
4. Next, it sends the extracted transcript to ChatGPT to generate a concise three-bullet point summary.
5. Finally, it compiles the video's title, the AI-generated summary, and the video link into a message.

## Output Details
The workflow posts a formatted message containing the new YouTube video's title, an AI-generated summary, and a direct link to the video on a specified Discord channel.

## Tags
automation, n8n, production-ready, excellent, optimized
