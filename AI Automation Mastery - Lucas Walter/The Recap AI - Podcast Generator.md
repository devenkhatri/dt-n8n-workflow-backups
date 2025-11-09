# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically creates a narrated podcast episode for 'Austin Daily Brief' by gathering local Austin event news from an RSS feed, extracting full article content, and using AI to craft and vocalize a concise and engaging script.

## Input Details
The workflow is manually triggered and starts by fetching an RSS feed containing links to Austin event news articles.

## Process Summary
The workflow begins by fetching an RSS feed of Austin event news. It then scrapes the full markdown content from all linked articles in a batch operation, polling until the scraping job completes. The collected article content is sent to Google Gemini AI, which generates a short, structured podcast script with annotations for ElevenLabs voice synthesis. The script includes specific tone, structure, and audio tag guidelines. Finally, the script is sent to ElevenLabs to produce a natural-sounding narrated MP3 podcast.

## Output Details
The workflow outputs an MP3 audio file of a narrated local events podcast, generated via the ElevenLabs text-to-speech API.

## Tags
podcast, AI, RSS, web scraping, text-to-speech, content generation, Austin, events, automation
