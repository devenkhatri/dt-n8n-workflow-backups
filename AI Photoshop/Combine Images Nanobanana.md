# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two images from Google Drive using an AI model (Nano Banana) based on a text prompt, then uploads the resulting image back to Google Drive and provides a shareable link.

## Input Details
The workflow is triggered by another workflow and receives a prompt, two Google Drive image file IDs, and a title for the output image.

## Process Summary
The workflow first formats the two input image IDs into an array and splits them into individual items. It downloads each image from Google Drive, uploads them to an image hosting service (IMGBB) to get public URLs, and aggregates those URLs. Using these URLs and the provided prompt, it sends a request to the Nano Banana AI service to generate a new combined image. The workflow then polls the AI service until the result is ready, downloads the generated image, uploads it to a specified Google Drive folder with the given title, and constructs a response message with the file name and Google Drive link.

## Output Details
The workflow outputs a message containing the name of the created image and its Google Drive sharing link.

## Tags
AI image generation, Google Drive, image processing, Nano Banana, IMGBB, workflow automation
