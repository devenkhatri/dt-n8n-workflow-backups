# Workflow Analysis for Googlesheets Workflow

## Description
This workflow automatically transcribes audio files uploaded to a specific Google Drive folder using AWS Transcribe and logs the transcription details into a Google Sheet.

## Input Details
The workflow is triggered when a new file is created in a specified Google Drive folder.

## Process Summary
When a file is added to the monitored Google Drive folder, it is uploaded to an AWS S3 bucket. AWS Transcribe is then used to create a transcription job for the audio file. The workflow waits for an external webhook to receive the transcription result. Once received, relevant details like transcription text, recording name, link, and timestamp are formatted and appended to a Google Sheet.

## Output Details
The transcription results and metadata are appended as a new row in a Google Sheet.

## Tags
Google Drive, AWS S3, AWS Transcribe, Google Sheets, audio transcription, automation, webhook, n8n
