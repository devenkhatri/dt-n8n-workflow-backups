# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow uses AI to edit an existing image based on a provided prompt, then saves the edited result to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives an image title, an image editing prompt, and a Google Drive file ID for the original image.

## Process Summary
The workflow downloads the original image from Google Drive using the provided file ID, uploads it to IMGBB to get a public URL, and sends this URL with the editing prompt to the Nano Banana AI service. It polls the AI service until the edited image is ready, downloads the result, and uploads it to a specific Google Drive folder. Finally, it constructs a response message containing the image name and a shareable Google Drive link.

## Output Details
The workflow outputs a message containing the name of the created image and a shareable link to view it in Google Drive.

## Tags
AI image editing, Google Drive, Nano Banana, image processing, workflow automation
