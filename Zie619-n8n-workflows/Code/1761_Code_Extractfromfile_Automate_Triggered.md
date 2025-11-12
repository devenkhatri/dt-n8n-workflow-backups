# Workflow Analysis for Automated Image Metadata Tagging

## Description
This workflow automatically analyzes images added to a Google Drive folder using AI to generate descriptive tags, then embeds those tags as metadata directly into the image file before saving it back to Google Drive.

## Input Details
The workflow is triggered when a new image file is added to a specific Google Drive folder.

## Process Summary
1. A Google Drive trigger detects when a new file is added to a specified folder. 2. The image file is downloaded from Google Drive. 3. The image is analyzed using an AI model (OpenAI) to generate a comma-separated list of descriptive tags. 4. The original image (as Base64) and the AI-generated tags are merged, and a custom code node embeds the tags into the image as XMP metadata. 5. The updated image with embedded metadata is converted back to a file and uploaded to replace the original in Google Drive.

## Output Details
The workflow updates the original image file in Google Drive with embedded XMP metadata containing AI-generated descriptive tags.

## Tags
automation, image processing, metadata tagging, Google Drive, AI analysis, OpenAI, XMP metadata, production-ready, n8n
