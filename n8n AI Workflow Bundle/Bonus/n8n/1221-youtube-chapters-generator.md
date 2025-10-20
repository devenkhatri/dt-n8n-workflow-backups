# Workflow Analysis for YouTube Chapters Generator

## Description
This workflow automates the creation of YouTube video chapters using AI. It takes a YouTube video URL, transcribes its audio, and then uses a large language model to generate time-stamped chapters based on the transcript. This workflow helps content creators quickly add structured navigation to their YouTube videos.

## Input Details
The workflow is triggered manually and receives a YouTube video URL as input.

## Process Summary
The workflow starts by extracting the YouTube video ID from the provided URL, then downloads the video's audio and transcribes it using an AI model. Next, it sends the transcript to another AI model with a prompt to generate YouTube chapters with timestamps. Finally, it formats the generated chapters into a readable form.

## Output Details
The workflow outputs a list of time-stamped YouTube chapters, which can be directly used in the YouTube video description.
