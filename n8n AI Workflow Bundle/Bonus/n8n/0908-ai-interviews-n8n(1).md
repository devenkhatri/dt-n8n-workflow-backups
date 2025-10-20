# Workflow Analysis for AI Interview Data Processing

## Description
This workflow automates the processing of AI interview data, including transcription, summarization, and saving relevant information to Google Sheets.

## Input Details
This workflow is manually triggered.

## Process Summary
The workflow starts by retrieving data from a Google Sheet. It then iterates through each row of data, transcribing the audio from a provided URL using an AI model. After transcription, it extracts the transcript and generates an interview summary. Finally, it formats the summary and updates the original Google Sheet with the generated transcript and summary.

## Output Details
The workflow updates a Google Sheet with the AI interview transcripts and summaries.
