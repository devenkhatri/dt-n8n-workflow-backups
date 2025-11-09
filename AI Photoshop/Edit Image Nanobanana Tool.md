# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an image using the Nano-Banana AI model based on a provided prompt. It downloads an existing image from Google Drive, sends it to an AI service for editing, uploads the resulting image back to Google Drive, and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives three inputs: imageTitle (name for the output file), imagePrompt (text instruction for editing the image), and imageID (Google Drive file ID of the original image).

## Process Summary
The workflow starts by downloading an image from Google Drive using the provided imageID. It then uploads this image to IMGBB to get a public URL. Using this URL and the provided image prompt, it sends a request to the Nano-Banana AI service to edit the image. The workflow waits 10 seconds and then polls the AI service for the result. Once the edited image is ready, it downloads the result, uploads it to a specific Google Drive folder with the provided title, and constructs a response message with the file name and Google Drive link.

## Output Details
The workflow produces a response message containing the name of the edited image and its Google Drive sharing link, which is passed back to the calling workflow.

## Tags
AI image editing, Google Drive integration, Nano-Banana, image processing, workflow automation
