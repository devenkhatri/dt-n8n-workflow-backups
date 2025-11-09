# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an existing image using the Nano-Banana AI model based on a provided text prompt, then uploads the result to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives three inputs: imageTitle (name for the output file), imagePrompt (text instruction for editing the image), and imageID (Google Drive ID of the original image).

## Process Summary
The workflow first downloads the original image from Google Drive using the provided image ID. It then uploads the image to IMGBB to get a public URL. Using this URL and the provided prompt, it sends a request to the Nano-Banana AI service to edit the image. The workflow polls the AI service until the edited image is ready, downloads the result, and uploads it to a specific Google Drive folder with the specified title. Finally, it constructs a response message with the file name and Google Drive link.

## Output Details
The workflow produces an edited image stored in Google Drive and returns a message containing the file name and a shareable Google Drive link to the edited image.

## Tags
AI Image Editing, Google Drive, Nano-Banana, Image Processing, Workflow Automation
