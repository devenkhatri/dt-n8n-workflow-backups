# Workflow Analysis for The Recap AI - Podcast Generator

## Description
This workflow automatically generates a short, engaging podcast episode about upcoming fun and non-controversial events in Austin. It pulls event data from an RSS feed, scrapes the full content from the event webpages, and then uses AI to write and narrate a professional-quality podcast script with expressive voice annotations.

## Input Details
The workflow is triggered manually and starts by fetching data from a predefined RSS feed containing Austin event information.

## Process Summary
The workflow begins by manually triggering a request to fetch an RSS feed of Austin events. It then sends the URLs from the feed to a web scraping service (Firecrawl) to extract the full content of each event page in markdown format. The workflow polls the scraping service until the job is complete or a retry limit is reached. Once the content is retrieved, it uses Google's Gemini AI model with a detailed prompt to generate a concise, engaging podcast script that includes ElevenLabs v3 audio tags for expressive narration. Finally, the script is sent to the ElevenLabs API to generate an MP3 audio file of the narrated podcast.

## Output Details
The workflow produces an MP3 audio file of a professionally narrated podcast episode about Austin events, generated via the ElevenLabs text-to-speech API.
