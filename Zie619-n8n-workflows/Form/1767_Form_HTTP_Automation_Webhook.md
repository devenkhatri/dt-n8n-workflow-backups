# Workflow Analysis for Youtube Video Transcript Extraction

## Description
This workflow allows users to submit a YouTube video URL and automatically retrieves and cleans the video's transcript for easy reading or further processing.

## Input Details
The workflow is triggered by a form submission containing a YouTube video URL.

## Process Summary
The workflow starts by accepting a YouTube video URL via a form. It then sends this URL to an external transcript extraction API using an HTTP request. The raw transcript data returned from the API is processed by a function node that handles different response formats, concatenates text segments, and cleans up spacing and punctuation. Finally, the cleaned transcript is structured into a standardized output format for use in downstream tasks.

## Output Details
The workflow outputs a cleaned and formatted transcript of the YouTube video, along with metadata such as video URL, duration, language, and offset.

## Tags
youtube, transcript, automation, n8n, video, text processing, production-ready, optimized
