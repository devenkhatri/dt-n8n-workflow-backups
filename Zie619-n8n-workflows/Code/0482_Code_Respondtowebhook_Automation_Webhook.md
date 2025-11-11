# Workflow Analysis for [n8n] YouTube Channel Advanced RSS Feeds Generator

## Description
This workflow generates multiple RSS feed formats for any public YouTube channel by accepting a channel username, channel ID, video URL, or video ID as input. It automatically detects the input type, resolves it to a channel ID, and produces 13 different RSS feed URLs—including video and community post feeds in various formats like HTML, JSON, Atom, MRSS, and more—without requiring a Google API key.

## Input Details
The workflow is triggered via a web form where the user submits a YouTube channel username, channel ID, video URL, or video ID.

## Process Summary
The workflow first validates and classifies the input (channel username, channel ID, or video ID). Depending on the input type, it retrieves the corresponding YouTube channel ID using third-party APIs. It then constructs a base XML RSS feed URL and generates multiple RSS feed variants using RSS Bridge for both videos and community posts in different formats (HTML, JSON, Atom, etc.). Finally, it combines and formats all feed URLs into an HTML table for response.

## Output Details
The workflow returns a formatted HTML table containing 13 unique RSS feed URLs (6 for videos, 6 for community posts, and 1 direct YouTube XML feed) as a webhook response.

## Tags
youtube, rss, automation, n8n, no-api, feed-generator, production-ready, optimized, third-party-api, xml
