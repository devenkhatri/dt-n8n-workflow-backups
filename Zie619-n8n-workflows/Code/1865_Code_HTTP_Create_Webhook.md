# Workflow Analysis for YT New Video Upload

## Description
This workflow automatically processes newly uploaded video files in a Google Drive folder by generating a transcript, creating an SEO-friendly title, writing a compelling description, and generating relevant YouTube tags—all using AI. It then uploads the video to YouTube as private and updates the video’s metadata with the generated content.

## Input Details
The workflow is triggered when a new file is added to a specific Google Drive folder, and it receives the file ID of the newly created file.

## Process Summary
The workflow starts by detecting a new file in a specified Google Drive folder. It downloads the video file, then sends it to an external service via HTTP request to generate a transcript. The transcript is reformatted into a single string and used as input for multiple AI models: one generates a YouTube description, another creates an SEO-optimized title, and a third produces relevant tags. The video is uploaded to YouTube as a private video, and its metadata (title, description, and tags) is updated using the AI-generated content. Optionally, the original file is deleted from the Drive folder after processing.

## Output Details
The workflow uploads the video to YouTube as a private video and updates its title, description, and tags using AI-generated content based on the video transcript.

## Tags
YouTube automation, Google Drive integration, AI content generation, video processing, transcript analysis, SEO optimization, n8n workflow, production-ready
