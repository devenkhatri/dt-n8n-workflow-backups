# Workflow Analysis for Zoom Meeting Assistant with AI Summary

## Description
This workflow acts as a smart assistant for Zoom meetings. It captures meeting recordings, transcribes them using AI, summarizes the transcript, and then shares the summary via email and Slack to relevant stakeholders, creating an automated meeting minute distribution system.

## Input Details
This workflow is triggered manually to start the process of fetching Zoom meeting details. It begins by retrieving information about Zoom meetings.

## Process Summary
First, the workflow identifies and processes new Zoom recordings, filtering to include only those with video files. It then downloads the video recording, uploads it to an AI transcription service to generate a transcript, and summarizes the transcript using another AI model. Finally, it formats the summary with key details such as meeting topic, duration, and attendees and distributes it.

## Output Details
The workflow sends the AI-generated meeting summary via email and posts it to a designated Slack channel. The AI-generated video transcript is outputted locally as a `mp3` file.
