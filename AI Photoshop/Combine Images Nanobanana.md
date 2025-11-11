# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two input images using an AI model (Nano Banana) based on a provided prompt, then uploads the resulting image to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives a prompt, two image file IDs from Google Drive, and a title for the output image.

## Process Summary
The workflow first restructures the input to create an array of the two image IDs, then splits them to download each image from Google Drive individually. Each downloaded image is uploaded to IMGBB to obtain public URLs. These URLs, along with the prompt, are sent to the Nano Banana AI service to generate a new combined image. The workflow polls the AI service until the result is ready, downloads the final image, uploads it to a specific Google Drive folder with the provided title, and constructs a response message with the file's name and link.

## Output Details
The workflow produces a Google Drive link to the newly created AI-generated image and returns a formatted response message containing the image name and link.

## Tags
AI Image Generation, Google Drive, Image Processing, Nano Banana, IMGBB, Workflow Automation
