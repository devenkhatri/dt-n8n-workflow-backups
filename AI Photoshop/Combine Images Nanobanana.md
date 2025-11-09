# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines two images using an AI model (Nano Banana) based on a provided text prompt, then uploads the resulting image to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered manually or by another workflow with input containing a prompt, two image file identifiers (image1 and image2), and a title for the output image.

## Process Summary
The workflow starts by receiving a prompt, two Google Drive image IDs, and a title. It downloads the two images from Google Drive, uploads them to IMGBB to get public URLs, then sends those URLs along with the prompt to the Nano Banana AI service to generate a new combined image. The workflow polls the AI service until the result is ready, downloads the resulting image, uploads it to a specific Google Drive folder with the given title, and finally constructs a response message with the image name and Google Drive link.

## Output Details
The workflow outputs a message containing the name of the generated image and its shareable Google Drive link.

## Tags
AI image generation, image combination, Google Drive, Nano Banana, IMGBB, HTTP request, workflow automation
