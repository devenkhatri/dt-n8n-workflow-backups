# Workflow Analysis for Tool - Generate Image

## Description
This workflow generates a custom image based on a provided context and title, following specific brand guidelines for The Recap AI Newsletter. It uses OpenAI's image generation API to create a watercolor-style image and shares it in a designated Slack channel.

## Input Details
The workflow is triggered manually or by another workflow and receives two inputs: 'imageContext' (a description for the image content) and 'imageTitle' (a title for the image).

## Process Summary
The workflow starts by setting predefined brand guidelines for image generation. It then sends a request to OpenAI's image generation API with the provided context and the brand guidelines as part of the prompt. The generated image, returned in base64 format, is converted into a PNG file. Finally, the workflow posts a message with the image title and uploads the generated image to a specific Slack channel.

## Output Details
The workflow outputs a generated image that is uploaded to a Slack channel along with a message containing the image title.

## Tags
image generation, OpenAI, Slack, brand guidelines, watercolor, marketing, AI
