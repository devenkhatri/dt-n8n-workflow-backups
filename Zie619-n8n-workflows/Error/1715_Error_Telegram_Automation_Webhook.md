# Workflow Analysis for template in store

## Description
This workflow automatically processes videos uploaded to a specific Google Drive folder by generating AI-powered social media descriptions and publishing the videos to both TikTok and Instagram. It uses OpenAI to transcribe audio from the video and create engaging captions based on successful examples, then uploads the video and description using the upload-post.com API.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder, receiving the file metadata and ID as input.

## Process Summary
When a new video file is detected in the Google Drive folder, the workflow downloads it and saves it locally. It then extracts audio from the video and sends it to OpenAI's GPT-4o model to generate a tailored social media description based on example captions. The workflow reads the saved video file twice—once for TikTok and once for Instagram—and uploads both the video and the AI-generated description to each platform using the upload-post.com API. Error handling is included to send Telegram notifications for failures, excluding specific DNS-related errors.

## Output Details
The workflow uploads the video along with its AI-generated description to both TikTok and Instagram via the upload-post.com API and sends error alerts to a Telegram chat when failures occur.

## Tags
automation, n8n, production-ready, excellent, optimized, google drive, openai, tiktok, instagram, social media automation, video processing, ai content generation
