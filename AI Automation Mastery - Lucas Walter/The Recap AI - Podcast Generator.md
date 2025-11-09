# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically generates a short, engaging podcast script about fun and interesting upcoming events in Austin, Texas, and then converts it into an audio file. It pulls event information from an RSS feed, scrapes the linked web pages for content, filters out controversial topics, and creates a professionally formatted script with voice annotations for natural-sounding narration.

## Input Details
The workflow is triggered manually and fetches event data from a specified RSS feed URL.

## Process Summary
The workflow starts by manually triggering a fetch of an RSS feed containing Austin event links. It then uses Firecrawl to batch-scrape the content from those URLs into markdown format, polling until the scraping is complete or retry limits are reached. Once the content is gathered, it uses Google's Gemini 2.5 Pro to generate a concise, engaging podcast script following specific guidelines for tone, structure, and ElevenLabs audio annotations. Finally, the generated script is sent to ElevenLabs to produce an MP3 audio file of the narrated podcast.

## Output Details
The workflow produces an audio file (MP3) of a narrated podcast about Austin events, generated via the ElevenLabs API.

## Tags
podcast,ai,austin,content-generation,text-to-speech,scraping,rss,automation
