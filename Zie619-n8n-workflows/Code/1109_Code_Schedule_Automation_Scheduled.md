# Workflow Analysis for YouTube to Airtable Anonym

## Description
This workflow automatically processes YouTube videos by extracting their transcripts, summarizing the content into a main idea and key takeaways, and storing the results in an Airtable base—streamlining content curation and idea management.

## Input Details
The workflow is triggered on a schedule (every minute) and fetches unprocessed YouTube video records from a specific Airtable table where the 'Status' is empty and 'Type' is 'Youtube Video'.

## Process Summary
The workflow starts by querying Airtable for new YouTube video entries. It extracts the video ID from the video URL using a code node. It then calls a third-party API via an HTTP request to fetch the transcript. The transcript data is parsed and combined into a single text string. This transcript is then passed to a summarization step (likely powered by an LLM, configured via a 'noOp' node acting as a placeholder for LLM instructions) that outputs a main idea and key takeaways. Finally, these insights are written back to the original Airtable record, and the 'Status' is updated to mark it as processed.

## Output Details
The workflow updates the original Airtable record with the extracted main idea, key takeaways, and marks the entry as processed by setting the 'Status' field.

## Tags
YouTube, Airtable, transcript, summarization, content curation, automation, n8n, production-ready, API integration, LLM
