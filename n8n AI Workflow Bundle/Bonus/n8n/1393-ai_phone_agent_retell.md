# Workflow Analysis for AI Phone Agent Retell

## Description
This workflow uses AI to analyze phone call recordings, summarize them, and extract key insights. It can be used for sales, customer service, or any business that relies on phone communications.

## Input Details
This workflow is triggered manually and does not receive any specific input data to start.

## Process Summary
The workflow begins by manually triggering. It then downloads an audio file from a specified URL, translates the audio into text using OpenAI Whisper, and stores the transcript in a text file. Subsequently, it summarizes the transcript and extracts key insights using OpenAI functions. Finally, the workflow saves the generated JSON output containing the summary and insights into an HTML file.

## Output Details
The workflow generates an HTML file containing the summary and key insights of the phone call and saves it.
