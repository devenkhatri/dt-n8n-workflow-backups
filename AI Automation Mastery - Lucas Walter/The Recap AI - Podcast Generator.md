# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically creates a short, engaging podcast about fun and interesting upcoming events in Austin, Texas, by gathering event data, generating a natural-sounding script with AI, and converting it into an audio file.

## Input Details
The workflow is manually triggered and receives event data by fetching from a specified Austin events RSS feed URL.

## Process Summary
The workflow begins by fetching an RSS feed of Austin events, then uses Firecrawl to scrape the content from each event's linked webpage into markdown. It employs Google's Gemini 2.5 Pro to generate a concise and engaging podcast script with specific tone, structure, and voice annotations for natural narration. The script is then sent to ElevenLabs to be converted into a narrated audio file. The process includes polling for scraping completion and implements retry logic for robustness.

## Output Details
The workflow produces an MP3 audio file of a narrated podcast about Austin events, generated through the ElevenLabs API.

## Tags
podcast,ai,austin,content-generation,text-to-speech,scraping,rss,automation
