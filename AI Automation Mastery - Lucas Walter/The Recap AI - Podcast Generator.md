# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically generates a narrated podcast episode for 'Austin Daily Brief' by fetching local event news from an RSS feed, scraping the full content of linked articles, and using AI to write and vocalize a concise, engaging script with natural-sounding narration.

## Input Details
The workflow is triggered manually and begins by fetching an RSS feed containing links to Austin event news articles.

## Process Summary
The workflow starts by manually triggering a fetch of an RSS feed. It then initiates a batch scrape of all article URLs from the feed to extract their full markdown content. The system polls the scrape job status until it completes or a retry limit is reached. Once scraping is successful, the combined article content is passed to a Google Gemini AI model, which writes a short, annotated podcast script following specific guidelines for tone, structure, and ElevenLabs audio tags. Finally, the generated script is sent to the ElevenLabs API to produce an MP3 audio file of the narrated podcast.

## Output Details
The workflow outputs a generated MP3 audio file of a narrated local events podcast, created via the ElevenLabs text-to-speech API.

## Tags
podcast, AI, RSS, web scraping, text-to-speech, content generation, Austin, events, automation
