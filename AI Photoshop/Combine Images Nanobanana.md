# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow takes two input images and a text prompt, combines the images using an AI image editing service (Nano Banana), and saves the resulting image to Google Drive with a custom title.

## Input Details
The workflow is triggered by another workflow and receives a text prompt, two Google Drive image file IDs, and an image title.

## Process Summary
The workflow first collects the two Google Drive image IDs and combines them into an array. It then downloads each image from Google Drive, uploads them to an image hosting service (IMGBB) to get public URLs, and sends those URLs along with the prompt to the Nano Banana AI service to generate a combined image. The workflow polls the AI service until the result is ready, downloads the final image, uploads it to a specified Google Drive folder with the given title, and constructs a response message with the file's web link.

## Output Details
The workflow outputs a message containing the name and Google Drive web link of the newly created combined image file.

## Tags
AI image generation, image editing, Google Drive, IMGBB, Nano Banana, workflow automation
