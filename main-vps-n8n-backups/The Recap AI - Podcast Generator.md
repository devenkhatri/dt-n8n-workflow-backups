# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically generates a short, engaging podcast script about upcoming fun and non-controversial events in Austin, based on an RSS feed of local news. It scrapes event webpages, uses an AI language model to write a human-like script with voice annotations, and sends the script to ElevenLabs to generate an audio file.

## Input Details
The workflow is triggered manually and begins by fetching data from a predefined RSS feed containing Austin event news.

## Process Summary
First, the workflow fetches an RSS feed of Austin events. It then sends the URLs from the feed to Firecrawl to scrape the full webpage content in markdown format. The system polls Firecrawl's API to check the scraping status, waiting 15 seconds between checks and retrying up to 30 times before failing. Once scraping is complete, the markdown content from all pages is combined. This combined content is passed to Google's Gemini 2.5 Pro model, which writes a podcast script following specific guidelines for tone, structure, and ElevenLabs audio tags. Finally, the generated script is sent to ElevenLabs' text-to-speech API to create an MP3 audio file.

## Output Details
The workflow produces an MP3 audio file of a narrated Austin events podcast by sending the AI-generated script to ElevenLabs' text-to-speech service.

## Tags
ai,podcast,rss,web scraping,elevenlabs,gemini,text-to-speech,content generation
