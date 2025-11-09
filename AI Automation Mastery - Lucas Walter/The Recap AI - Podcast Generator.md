# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically generates a short, engaging podcast script about upcoming fun and non-controversial events in Austin by pulling data from an RSS feed, scraping the linked web pages for content, and using AI to write and narrate a production-ready audio brief.

## Input Details
The workflow is triggered manually and fetches event data from a predefined RSS feed URL.

## Process Summary
The workflow starts by manually triggering a request to fetch an RSS feed containing event links. It then initiates a batch scrape of all linked pages using Firecrawl to extract clean markdown content. The system polls the scrape job status, waiting until completion or until a retry limit is reached. Once scraping is successful, the extracted content is passed to a Google Gemini AI model, which writes a concise, annotated podcast script following specific guidelines for tone, structure, and ElevenLabs audio tags. Finally, the generated script is sent to ElevenLabs to produce an MP3 audio file of the narrated podcast.

## Output Details
The workflow produces a narrated MP3 audio file of a short podcast about Austin events via the ElevenLabs text-to-speech API.

## Tags
podcast, AI, content-generation, web-scraping, rss, elevenlabs, gemini, automation, audio-generation, austin-events
