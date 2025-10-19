# Workflow Analysis for YouTube Transcript Downloader and Summarizer

## Description
This workflow automates the process of extracting transcripts from YouTube videos, summarizing them, and saving both the original transcript and the summary to a specified Google Drive folder.

## Input Details
The workflow is triggered manually and receives a YouTube video URL as input.

## Process Summary
The workflow starts by taking a YouTube video URL. It then extracts the transcript of the video using a custom Python script. Next, it sends this transcript to an OpenAI GPT model for summarization. Finally, both the original transcript and the generated summary are uploaded to a designated Google Drive folder.

## Output Details
The workflow outputs two text files to Google Drive: one containing the full YouTube video transcript and another with its summary.
