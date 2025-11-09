# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow intelligently merges two images using AI (Nano Banana) based on a provided text prompt, then stores the result in Google Drive and returns a shareable link.

## Input Details
Triggered by another workflow, it receives a text prompt, two Google Drive file IDs for source images, and a title for the output image.

## Process Summary
The workflow downloads two images from Google Drive using their file IDs, uploads them to IMGBB to get public URLs, and sends these URLs along with a text prompt to the Nano Banana AI service. It polls Nano Banana until the combined image is ready, downloads the result, and uploads it to a designated Google Drive folder with the specified title. Finally, it constructs a response message with the file name and shareable Google Drive link.

## Output Details
Returns a message containing the name and shareable Google Drive web link of the newly created combined image file.

## Tags
AI image generation, image editing, Google Drive, IMGBB, Nano Banana, workflow automation
