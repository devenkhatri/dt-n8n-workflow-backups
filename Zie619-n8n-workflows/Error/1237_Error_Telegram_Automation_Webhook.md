# Workflow Analysis for Google Drive to Instagram, TikTok and YouTube

## Description
This workflow automatically uploads videos added to a specific Google Drive folder to Instagram, TikTok, and YouTube, complete with AI-generated captions tailored for each platform.

## Input Details
The workflow is triggered when a new file is added to a designated Google Drive folder.

## Process Summary
When a new video file is detected in the specified Google Drive folder, the workflow downloads the file and saves it locally. It then uses OpenAI to transcribe the video audio and generate an engaging social media description based on the transcript. The original video is read back from local storage and uploaded simultaneously to Instagram, TikTok, and YouTube via the upload-post.com API, using the generated description (truncated for YouTube's title limits). Error handling is included to notify a Telegram channel if something goes wrong during the process, excluding certain DNS-related errors.

## Output Details
The workflow uploads the video with an AI-generated description to Instagram, TikTok, and YouTube, and sends error alerts to a Telegram channel if failures occur.

## Tags
social media automation, video upload, Google Drive, Instagram, TikTok, YouTube, AI description, OpenAI, n8n, upload-post.com
