# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow takes two input images and a text prompt, combines them using an AI image generation service called Nano-Banana, and saves the resulting image to a specified Google Drive folder with a custom title.

## Input Details
The workflow is triggered by another workflow and receives a text prompt, two image file IDs from Google Drive, and a title for the output image.

## Process Summary
The workflow first structures the two input image IDs into an array and splits them into separate items. It then downloads each image from Google Drive and uploads them to IMGBB to obtain public URLs. These URLs, along with the provided prompt, are sent to the Nano-Banana AI service to generate a new combined image. The workflow polls the AI service until the result is ready, downloads the generated image, and uploads it to a designated Google Drive folder using the provided title.

## Output Details
The workflow uploads the AI-generated image to Google Drive and returns a message containing the file name and a direct link to the uploaded image.

## Tags
AI Image Generation, Google Drive, Image Processing, Nano-Banana, Workflow Integration
