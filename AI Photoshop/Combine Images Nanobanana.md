# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow uses AI to combine two images based on a text prompt and saves the result to Google Drive.

## Input Details
Triggered by another workflow, it receives a text prompt, two Google Drive image file IDs, and a desired output image title.

## Process Summary
The workflow downloads two images from Google Drive using their file IDs and uploads them to IMGBB to obtain public URLs. It then sends these URLs along with a text prompt to the Nano-Banana AI service to generate a combined image. The workflow polls the AI service until the result is ready, downloads the generated image, and uploads it to a specified Google Drive folder with the provided title.

## Output Details
The AI-generated combined image is uploaded to Google Drive, and the workflow returns a message containing the file name and a link to the image in Google Drive.

## Tags
AI Image Generation, Image Editing, Google Drive, Nano-Banana, Image Processing, Workflow Automation
