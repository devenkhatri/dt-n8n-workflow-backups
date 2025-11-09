# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow uses AI to merge two images from Google Drive using a text prompt and saves the result back to Google Drive with a custom title.

## Input Details
Triggered by another workflow, it receives a text prompt, two Google Drive image file IDs, and a custom title for the output image.

## Process Summary
The workflow downloads two images from Google Drive using their file IDs and uploads them to IMGBB to get public URLs. It then sends these URLs along with a text prompt to the Nano-Banana AI service to generate a combined image. The workflow polls Nano-Banana until the result is ready, then downloads the generated image. Finally, it uploads the resulting image to a specified Google Drive folder using the provided custom title.

## Output Details
The workflow uploads the AI-generated image to Google Drive and returns a message with the file name and a direct link to the uploaded image.

## Tags
AI Image Generation, Google Drive, Image Processing, Nano-Banana, Workflow Integration
