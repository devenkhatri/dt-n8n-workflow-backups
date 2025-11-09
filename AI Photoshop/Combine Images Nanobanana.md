# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two images using the Nano Banana AI model based on a text prompt, then uploads the result to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered manually or by another workflow with a text prompt, two Google Drive image file IDs, and a title for the output image.

## Process Summary
The workflow downloads two images from Google Drive using provided file IDs, uploads them to IMGBB to obtain public URLs, and sends these URLs along with a user-provided prompt to the Nano Banana AI service. It then polls the AI service until the combined image is ready, downloads the result, uploads it to a specified Google Drive folder with the given title, and generates a shareable link.

## Output Details
The workflow returns a message containing the name of the generated image and its shareable Google Drive link.

## Tags
AI image generation, image combination, Google Drive, Nano Banana, IMGBB, HTTP request, workflow automation
