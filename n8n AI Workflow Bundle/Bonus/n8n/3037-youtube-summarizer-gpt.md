# Workflow Analysis for YouTube Video Summarizer using GPT

## Description
This workflow summarizes YouTube videos using OpenAI's GPT models, providing a concise overview of video content.

## Input Details
This workflow is manually triggered and takes a YouTube video URL as input.

## Process Summary
First, the workflow extracts the video ID and uses it to retrieve the video transcript from YouTube. Then, it chunks the transcript into manageable segments and uses the OpenAI GPT-3.5 model to summarize each segment. Finally, it combines these summaries and generates a comprehensive summary of the entire video using the GPT-3.5 model again.

## Output Details
The workflow outputs a concise summary of the YouTube video.
