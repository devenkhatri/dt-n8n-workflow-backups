# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an existing image using the Nano Banana AI model based on a provided prompt, then saves the result to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives three inputs: an image title, an image editing prompt, and a Google Drive file ID for the original image.

## Process Summary
The workflow first downloads the original image from Google Drive using the provided file ID. It then uploads the image to IMGBB to get a public URL. Using this URL and the provided prompt, it sends a request to the Nano Banana AI service to edit the image. The workflow polls the AI service until the result is ready, downloads the edited image, and uploads it to a specific Google Drive folder. Finally, it constructs a response message with the image name and Google Drive link.

## Output Details
The workflow outputs a message containing the name of the created image and a link to view it in Google Drive.

## Tags
AI image editing, Google Drive, Nano Banana, image processing, workflow automation
