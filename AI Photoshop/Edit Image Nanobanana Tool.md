# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an existing image using the Nano Banana AI model based on a provided prompt, then saves the result to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives an image title, an image editing prompt, and a Google Drive file ID for the original image.

## Process Summary
The workflow downloads the original image from Google Drive using the provided file ID, then uploads it to IMGBB to obtain a public URL. It sends this URL along with the editing prompt to the Nano Banana AI service to generate an edited image. The workflow polls the AI service until the result is ready, then downloads the edited image. Finally, it uploads the edited image to a specific Google Drive folder and constructs a response message with the image name and Google Drive link.

## Output Details
The workflow outputs a message containing the name of the created image and a shareable link to view it in Google Drive.

## Tags
AI image editing, Google Drive, Nano Banana, image processing, workflow automation
