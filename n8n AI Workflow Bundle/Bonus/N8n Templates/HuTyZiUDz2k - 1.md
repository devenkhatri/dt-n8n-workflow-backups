# Workflow Analysis for AI-Powered YouTube Shorts Creator with Pexels, ElevenLabs, and VIDDS

## Description
This workflow automates the creation of a YouTube Short video. It starts by generating a compelling script using OpenAI, which is then converted into a voice-over audio file using ElevenLabs. Concurrently, it finds a high-quality stock video from Pexels, downloads both the video and audio, and uploads them to an AWS S3 bucket. Finally, it uses the VIDDS service to combine the video and audio into a complete, rendered YouTube Short, and sends the final video link via a Telegram notification.

## Input Details
The workflow is triggered by an external Webhook (HTTP GET request), which initiates the entire video creation process.

## Process Summary
The workflow uses OpenAI to generate a video script and ElevenLabs to convert that script into an MP3 audio file. Concurrently, it selects a random video from a curated list of Pexels videos, extracts its 1080p link, and downloads the raw video file. Both the audio and video files are uploaded to an AWS S3 bucket. A request is sent to VIDDS to create a video project combining the S3 assets and initiate rendering. The workflow then waits and polls VIDDS until the video status is "RENDERED" before extracting the final video URL and sending it to Telegram.

## Output Details
The workflow produces a finished, rendered MP4 video (a YouTube Short) and sends the final public URL of this video to a specified Telegram chat.
