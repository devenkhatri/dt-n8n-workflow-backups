# Workflow Analysis for 🎥 Analyze YouTube Video for Summaries, Transcripts & Content + Google Gemini AI

## Description
This workflow analyzes a YouTube video using Google's Gemini AI to generate tailored content such as summaries, transcripts, scene descriptions, or social media clips based on user-selected prompt types. It first gathers video metadata, then uses that context to construct precise AI prompts, and finally returns the AI-generated results in multiple formats including HTML, email, and Google Drive.

## Input Details
The workflow is triggered by a user submitting a form with a YouTube video ID and a selected prompt type (e.g., summary, transcript, clips).

## Process Summary
1. The workflow starts by collecting the YouTube video ID and prompt type via a form. 2. It fetches basic video details from the YouTube Data API. 3. It sends the video to Google Gemini AI with a meta-prompt to extract audience and content metadata (like video type, key topics, tone, etc.). 4. Using this metadata, it dynamically selects and composes a tailored prompt based on the user’s selected prompt type (e.g., summary, transcribe, scene). 5. The composed prompt and video are sent to Gemini again to generate the final AI output, which is then formatted and delivered via HTML, email, and Google Drive.

## Output Details
The workflow outputs AI-generated content (summary, transcript, etc.) as an HTML response to the user, saves it as a text file in Google Drive, and emails it via Gmail.

## Tags
YouTube, Google Gemini, AI, transcription, summarization, content analysis, automation, n8n, Google Drive, Gmail, video analysis
