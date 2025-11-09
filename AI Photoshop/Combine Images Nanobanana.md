# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow uses the Nano-Banana AI service to combine two input images based on a text prompt, then saves the resulting image to a specified Google Drive folder with a custom title.

## Input Details
Triggered by another workflow, it receives a text prompt, two Google Drive image file IDs, and a desired output image title.

## Process Summary
The workflow collects the two Google Drive image IDs and downloads the images. It uploads them to IMGBB to get public URLs, then sends those URLs along with the text prompt to the Nano-Banana AI service. It polls the AI service until the combined image is ready, downloads the result, and uploads it to a designated Google Drive folder using the provided title.

## Output Details
The AI-generated combined image is uploaded to Google Drive, and the workflow returns a message containing the file name and a link to the image in Google Drive.

## Tags
AI Image Generation, Image Editing, Google Drive, Nano-Banana, Image Processing, Workflow Automation
