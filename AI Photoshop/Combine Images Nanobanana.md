# Workflow Analysis for AI Image Combination and Google Drive Storage

## Description
This workflow combines two input images using an AI model based on a provided text prompt, then saves the resulting AI-generated image to Google Drive.

## Input Details
This workflow is triggered by another workflow, receiving a text prompt, two Google Drive image IDs, and a desired title for the output image.

## Process Summary
The workflow first retrieves two specified images from Google Drive. It then uploads these images to imgbb.com to generate public URLs. These URLs, along with the user-provided prompt, are sent to the Fal.ai Nano Banana service to create a new AI-edited image. The workflow polls the Fal.ai service periodically until the image generation is complete, then downloads the final image. Finally, the generated image is uploaded to a designated Google Drive folder with the specified title.

## Output Details
The workflow uploads the newly generated AI image to a Google Drive folder and provides a confirmation message including the Google Drive shareable link.
