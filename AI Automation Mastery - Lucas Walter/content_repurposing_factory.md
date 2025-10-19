# Workflow Analysis for Content Repurposing Factory

## Description
This workflow automates the repurposing of content by taking a YouTube video, transcribing it, generating various content formats like blog posts, tweets, and LinkedIn posts, and then saving them to Google Drive.

## Input Details
The workflow is triggered manually and receives a YouTube video URL as input.

## Process Summary
The workflow starts by extracting the YouTube video ID and then transcribing the video to text. It then uses AI to generate a blog post, a tweet, a LinkedIn post, and a short text summary from the transcript. Finally, it combines all the generated content into a single JSON object.

## Output Details
The repurposed content in JSON format is saved to Google Drive.
