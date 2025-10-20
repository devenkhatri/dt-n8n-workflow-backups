# Workflow Analysis for AI Short-Form Video Generator

## Description
This workflow automates the creation of short-form marketing videos leveraging AI for script generation, speech synthesis, and video production.

## Input Details
This workflow is manually triggered or initiated via a webhook, receiving text input for video content.

## Process Summary
The workflow starts by rewriting the input text into a concise short-form video script using OpenAI. This refined script is then used to generate voice narration via ElevenLabs. Subsequently, the script and narration are sent to Pictory.ai to produce a video, which includes visual media and text overlays. Finally, the generated video file is uploaded to Google Drive for storage and accessibility.

## Output Details
The workflow produces a short-form marketing video and stores it in Google Drive, making it accessible via a shareable link.
