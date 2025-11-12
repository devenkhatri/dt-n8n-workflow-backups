# Workflow Analysis for Podcast Digest

## Description
This workflow automatically processes a podcast episode transcript to generate a structured digest that includes a summary, key topics, and thought-provoking questions. It then enriches each topic with background information from Wikipedia and emails the final HTML-formatted digest to a specified recipient.

## Input Details
The workflow is triggered manually and receives a hardcoded podcast episode transcript as input.

## Process Summary
The workflow starts by loading a podcast transcript, then splits it into manageable chunks. It uses GPT-3.5 to summarize the transcript via a refine method. From the summary, GPT-4 extracts structured lists of relevant topics and questions. Each topic is then researched using a GPT-3.5-powered agent with access to Wikipedia. Finally, all components—summary, enriched topics, and questions—are formatted into an HTML email digest.

## Output Details
The workflow sends a rich HTML email digest containing the episode summary, explained topics, and reflective questions to a predefined Gmail address.

## Tags
podcast, digest, summarization, GPT, automation, email, n8n, philosophy, consciousness, illusionism
