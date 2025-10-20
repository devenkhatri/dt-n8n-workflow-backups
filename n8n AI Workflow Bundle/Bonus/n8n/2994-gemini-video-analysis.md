# Workflow Analysis for Gemini Video Analysis from Webhook and Upload to Google Drive

## Description
This workflow analyzes video content by extracting frames, generating descriptions using AI, and then storing these descriptions in a Google Sheet and uploading the frames to Google Drive.

## Input Details
The workflow is triggered by a webhook and receives video file data along with a prompt to analyze the video.

## Process Summary
The workflow starts by receiving a video file and an analysis prompt via a webhook. It then extracts frames from the video at a specified interval. For each extracted frame, it converts the image to base64 and uses the Google Gemini AI model to generate a description based on the provided prompt and the image. These descriptions, along with the original video name, frame number, and prompt, are then added as new rows to a specified Google Sheet. Finally, each extracted video frame is uploaded to a designated folder in Google Drive.

## Output Details
The workflow outputs video frame descriptions to a Google Sheet and uploads the extracted video frames to Google Drive.
