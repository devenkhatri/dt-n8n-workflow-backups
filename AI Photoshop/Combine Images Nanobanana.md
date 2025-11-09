# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two input images using AI-powered image editing (Nano Banana) based on a text prompt, then saves the resulting image to Google Drive with a custom title and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives a text prompt, two Google Drive image file IDs, and an image title.

## Process Summary
The workflow collects two Google Drive image IDs and downloads the images. It uploads them to IMGBB to obtain public URLs, then sends these URLs along with a text prompt to the Nano Banana AI service to generate a combined image. The workflow polls Nano Banana until the result is ready, downloads the final image, and uploads it to a specified Google Drive folder with the provided title. Finally, it constructs a response message containing the file's name and web link.

## Output Details
The workflow outputs a message containing the name and Google Drive web link of the newly created combined image file.

## Tags
AI image generation, image editing, Google Drive, IMGBB, Nano Banana, workflow automation
