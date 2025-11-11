# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an existing image using AI based on a provided prompt. It downloads the original image from Google Drive, sends it to an AI image editing service (Nano Banana via Fal.ai), waits for the result, downloads the edited image, uploads it back to Google Drive, and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives three inputs: imageTitle (name for the output image), imagePrompt (text instruction for editing the image), and imageID (Google Drive file ID of the original image).

## Process Summary
The workflow starts by downloading the original image from Google Drive using the provided imageID. It then uploads this image to IMGBB to get a public URL. Using this URL and the provided imagePrompt, it sends a request to the Nano Banana AI image editing API. After waiting 10 seconds, it polls the API for results, repeating if needed. Once the edited image is ready, it downloads the result, uploads it to a specific Google Drive folder with the provided imageTitle, and prepares a response message with the file's shareable link.

## Output Details
The workflow produces a response message containing the name of the edited image and a Google Drive link to view it, which is passed back to the calling workflow.

## Tags
AI Image Editing, Google Drive, Fal.ai, Nano Banana, Image Processing, File Upload, HTTP Request, Workflow Integration
