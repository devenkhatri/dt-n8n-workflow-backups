# Workflow Analysis for Zoom AI Meeting Automation

## Description
This workflow automates the processing of Zoom meeting recordings by transcribing them, summarizing the content using AI, and then storing the output in Google Drive.

## Input Details
The workflow is triggered by new Zoom meeting recordings via a webhook.

## Process Summary
The workflow starts when a new Zoom meeting recording is available. It then retrieves the recording ID and downloads the audio file. The audio is transcribed using AssemblyAI, and the transcript is sent to OpenAI for summarization. Finally, the meeting summary is saved as a text file in Google Drive, and the transcribed text is also saved as a text file in Google Drive.

## Output Details
The workflow produces a summarized text file and a full transcript file of the Zoom meeting, both stored in Google Drive.
