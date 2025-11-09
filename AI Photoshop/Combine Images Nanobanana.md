# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two input images using an AI model (Nano Banana) based on a provided text prompt, then saves the resulting image to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives a prompt, two image file identifiers (from Google Drive), and an image title.

## Process Summary
The workflow first collects the two input image IDs and splits them into individual items. It then downloads each image from Google Drive and uploads them to IMGBB to get public URLs. These URLs, along with the text prompt, are sent to the Nano Banana AI API to generate a new combined image. The workflow polls the AI service until the result is ready, downloads the final image, uploads it to a specific Google Drive folder with the provided title, and constructs a response message with the file's name and web link.

## Output Details
The workflow outputs a message containing the name and Google Drive web link of the newly created AI-generated image.

## Tags
AI image generation, image combining, Google Drive, Nano Banana, IMGBB, workflow automation
