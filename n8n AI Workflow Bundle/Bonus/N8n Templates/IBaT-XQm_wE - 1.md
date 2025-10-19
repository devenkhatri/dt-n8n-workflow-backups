# Workflow Analysis for YouTube Video Transcription and Summary via OpenAI

## Description
This workflow automates the process of extracting information from a YouTube video. It downloads the video's audio, uses OpenAI's Whisper model to generate a complete transcription, and then leverages a large language model (LLM) like GPT to create a concise summary of the transcribed content.

## Input Details
The workflow is initiated via a manual trigger and requires a YouTube video URL as input.

## Process Summary
The workflow first takes a YouTube URL and downloads the necessary audio/video data via an HTTP request. It then sends this file to the OpenAI Whisper model to generate a full text transcription. Next, the full transcription is passed to a GPT model to create a short, digestible summary. The final step organizes the video's title, the full transcription, and the summary into a single output.

## Output Details
The final output is a structured object containing the YouTube video title, the complete text transcription, and the AI-generated summary.
