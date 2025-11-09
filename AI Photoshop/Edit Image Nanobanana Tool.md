# Workflow Analysis for Edit Image Nanobanana Tool

## Description
This workflow edits an existing image using an AI-powered image editing service (Nano Banana) based on a provided prompt, then saves the edited image to Google Drive and returns a shareable link.

## Input Details
The workflow is triggered by another workflow and receives three inputs: imageTitle (name for the edited image), imagePrompt (text description of the desired edit), and imageID (Google Drive file ID of the original image).

## Process Summary
The workflow starts by downloading the original image from Google Drive using the provided imageID. It then uploads the image to IMGBB to get a public URL. Using this URL and the provided prompt, it sends a request to the Nano Banana AI service to edit the image. The workflow polls the Nano Banana service every 5-10 seconds until the edited image is ready. Once available, it downloads the edited image and uploads it to a specific folder in Google Drive with the provided title.

## Output Details
The workflow produces a message containing the name of the edited image and a shareable Google Drive link to the edited image file.

## Tags
AI,image editing,Google Drive,IMGBB,Nano Banana,image generation
