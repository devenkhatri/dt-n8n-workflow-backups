# Workflow Analysis for Daily Meeting Summarization with Gemini AI

## Description
This workflow automates the summarization of daily meeting transcripts using Google's Gemini AI and sends the summary to a Discord channel.

## Input Details
The workflow is triggered manually.

## Process Summary
First, the workflow retrieves meeting transcripts from a Google Drive folder. Next, it iterates through each transcript, extracts the content, and sends it to the Gemini AI model for summarization. The summarized content is then formatted and sent as a message to a designated Discord channel. Finally, the workflow marks the processed meeting transcripts as moved to prevent redundant processing.

## Output Details
The workflow outputs summarized meeting notes to a specified Discord channel.
