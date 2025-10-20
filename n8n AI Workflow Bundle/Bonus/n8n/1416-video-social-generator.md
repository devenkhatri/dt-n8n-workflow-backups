# Workflow Analysis for Video Social Generator

## Description
This workflow generates social media posts based on video content. It fetches video data, transcribes the audio, generates summaries and hashtags, and then creates image posts for various social media platforms.

## Input Details
The workflow is triggered manually and receives video URLs as input.

## Process Summary
The workflow starts by fetching video metadata from a provided URL. It then uses an AI model to transcribe the video audio. Following transcription, another AI model summarizes the transcription and extracts relevant keywords and hashtags. Finally, the workflow generates distinct image posts for Facebook, Instagram, LinkedIn, and Twitter, incorporating the video thumbnail, title, summary, and hashtags.

## Output Details
The workflow outputs image posts tailored for Facebook, Instagram, LinkedIn, and Twitter, which can be then published to their respective platforms.
