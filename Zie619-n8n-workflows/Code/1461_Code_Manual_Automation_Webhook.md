# Workflow Analysis for YouTube Video Analyzer with AI

## Description
This workflow automatically analyzes YouTube videos by extracting their transcripts using an external API, processes the full transcript text, and uses AI models to generate a structured summary with a descriptive title. The final analysis is then emailed to a specified recipient.

## Input Details
The workflow is triggered manually and receives a YouTube video URL via an environment variable (WEBHOOK_URL).

## Process Summary
The workflow starts by setting the YouTube URL from an environment variable, then extracts the video ID from the URL using regex. It sends a request to an external transcript API to fetch the video's transcript. If a transcript exists, it combines all transcript segments into a single text string. This full text is then analyzed by an AI language model (with options for OpenAI, OpenRouter, or DeepSeek) following specific formatting instructions to produce a structured summary and title. Finally, the result is sent via email.

## Output Details
The workflow sends an email containing the AI-generated title as the subject and the structured video analysis as the body text.

## Tags
YouTube, video analysis, AI, transcript extraction, email automation, OpenAI, DeepSeek, OpenRouter, n8n, production-ready
