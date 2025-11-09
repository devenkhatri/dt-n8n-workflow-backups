# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two input images with a text prompt using the Nano-Banana AI image generation service and saves the resulting image to Google Drive with a custom title.

## Input Details
The workflow is triggered by another workflow and receives a text prompt, two Google Drive image file IDs, and a title for the output image.

## Process Summary
The workflow structures the two Google Drive image file IDs into an array and processes them individually. Each image is downloaded from Google Drive and uploaded to IMGBB to generate public URLs. These URLs and the provided text prompt are sent to the Nano-Banana AI service to generate a combined image. The workflow polls Nano-Banana until the result is ready, downloads the generated image, and uploads it to a specified Google Drive folder using the provided title.

## Output Details
The workflow uploads the AI-generated image to Google Drive and returns a message with the file name and a direct link to the uploaded image.

## Tags
AI Image Generation, Google Drive, Image Processing, Nano-Banana, Workflow Integration
