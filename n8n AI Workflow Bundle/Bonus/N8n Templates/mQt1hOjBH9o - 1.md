# Workflow Analysis for Automated Article to Video Creation with AI Voiceover

## Description
This workflow automates the process of converting an article into a video, complete with AI-generated voiceover, and then uploads it to YouTube. It orchestrates various AI services to create a complete video from a given article URL.

## Input Details
This workflow is triggered manually and requires an article URL as input.

## Process Summary
The workflow starts by extracting content from the provided article URL. Then, it uses an AI model to generate a video script from the article content, which is subsequently used to create image prompts. These prompts are then used to generate images. An AI service creates an audio voiceover from the video script. Finally, the generated audio and images are combined to create the video.

## Output Details
The workflow uploads the generated video to YouTube.
