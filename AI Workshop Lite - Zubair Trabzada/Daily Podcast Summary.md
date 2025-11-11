# Workflow Analysis for Daily Podcast Summary

## Description
This workflow fetches the top podcast episodes in a specified genre, downloads and trims each episode to a manageable segment, transcribes the audio using OpenAI's Whisper, summarizes the content with GPT, and emails a formatted HTML report with links and summaries to the user.

## Input Details
The workflow is triggered on a daily schedule (defaulting to 8 AM) and receives no external input data beyond the configured genre and API credentials.

## Process Summary
The workflow starts by fetching the top podcast episodes in a specified genre (e.g., TECHNOLOGY) from the Taddy API. Each episode's audio is downloaded and sent to an audio cropping service to extract a segment (8-24 minutes). Once the cropped audio is ready, it is downloaded and transcribed using OpenAI's Whisper. The resulting transcript is then summarized using GPT-4o-mini. Finally, all podcast summaries are compiled into an HTML email and sent via Gmail.

## Output Details
The workflow produces a daily HTML email containing podcast names, links to the audio, and AI-generated summaries, which is sent to the user's configured Gmail address.

## Tags
podcast, summary, email, automation, OpenAI, Whisper, transcription, daily digest, audio processing, Taddy
