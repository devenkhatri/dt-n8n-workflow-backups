# Workflow Analysis for Automate Instagram Posts with Google Drive, AI Captions & Facebook Graph API

## Description
This workflow automatically posts content to Instagram when a new photo, video, or carousel is added to a designated Google Drive folder. It uses AI to generate engaging captions, logs post details in Google Sheets, and publishes the content via Facebook's Graph API.

## Input Details
The workflow is triggered when a new file is uploaded to a specific Google Drive folder.

## Process Summary
1. A new file upload in a Google Drive folder triggers the workflow.
2. The file is downloaded into the n8n environment.
3. OpenAI generates an engaging Instagram caption based on the file name.
4. The file details, caption, and thumbnail are saved to a Google Sheet for record-keeping.
5. The Facebook Graph API is used to publish the media as an Instagram Reel with the AI-generated caption.

## Output Details
The workflow publishes the media file as an Instagram Reel with an AI-generated caption and saves a record of the post in Google Sheets.

## Tags
Instagram automation, Google Drive, OpenAI, Facebook Graph API, social media posting, AI caption generator, Google Sheets, n8n workflow
