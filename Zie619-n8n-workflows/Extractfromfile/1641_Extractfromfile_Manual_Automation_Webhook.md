# Workflow Analysis for YouTube Chapter Generator

## Description
This workflow automatically generates timestamped chapters for a YouTube video based on its captions and updates the video description with these chapters.

## Input Details
The workflow is triggered manually and starts with a predefined YouTube video ID.

## Process Summary
The workflow begins by setting a specific YouTube video ID. It then retrieves the video's metadata and caption ID via YouTube API calls. Using the caption ID, it fetches the actual captions (in SRT format), extracts the text content, and sends it to Google Gemini AI to generate structured chapter timestamps. Finally, it updates the video's description on YouTube by appending the generated chapters.

## Output Details
The workflow updates the YouTube video’s description with auto-generated chapters based on its transcript.

## Tags
YouTube, automation, AI, video chapters, captions, Google Gemini, n8n, production-ready
