# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an image using the Nano-Banana AI model based on a text prompt. It retrieves an image from Google Drive, processes it with AI, and saves the result back to Google Drive with a shareable link.

## Input Details
Triggered by another workflow with inputs: imageTitle (output file name), imagePrompt (editing instruction), and imageID (Google Drive file ID of the source image).

## Process Summary
The workflow downloads an image from Google Drive using the provided file ID, uploads it to IMGBB to obtain a public URL, and sends this URL along with the editing prompt to the Nano-Banana AI service. After waiting 10 seconds, it polls the AI service until the edited image is ready. Once available, it downloads the result, uploads it to a specified Google Drive folder using the provided title, and generates a shareable Google Drive link.

## Output Details
Returns a response message containing the edited image's file name and its Google Drive sharing link to the calling workflow.

## Tags
AI image editing, Google Drive integration, Nano-Banana, image processing, workflow automation
