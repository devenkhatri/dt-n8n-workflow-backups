# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two input images using an AI image editing service called Nano-Banana, based on a provided text prompt, and saves the resulting image to a specific Google Drive folder with a custom title.

## Input Details
The workflow is triggered by another workflow and receives a text prompt, two image file identifiers (for Google Drive), and a title for the output image.

## Process Summary
The workflow first collects the two image identifiers and combines them into an array. It then downloads each image from Google Drive and uploads them to IMGBB to obtain public URLs. Using these URLs and the provided prompt, it sends a request to the Nano-Banana AI service to generate a new combined image. The workflow polls the AI service until the result is ready, downloads the final image, and uploads it to a designated Google Drive folder with the specified title.

## Output Details
The workflow uploads the AI-generated combined image to a Google Drive folder and produces a response message containing the file name and a link to the image in Google Drive.

## Tags
AI Image Generation, Image Editing, Google Drive, Nano-Banana, Image Processing, Workflow Automation
