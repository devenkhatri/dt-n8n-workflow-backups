# Workflow Analysis for Transform Image to Lego Style Using Line and Dall-E

## Description
This workflow automatically transforms an image sent via LINE messenger into a LEGO-style image using AI. It receives the image through a LINE webhook, analyzes it to generate a suitable prompt, creates a LEGO version using DALL·E, and sends the result back to the user through LINE.

## Input Details
The workflow is triggered by a POST request to a LINE webhook containing an image message from a user.

## Process Summary
The workflow starts by receiving an image via a LINE webhook. It then fetches the message content from LINE's API. Using OpenAI's vision model, it generates a prompt that describes how to convert the image into an isometric LEGO-style version. This prompt is passed to DALL·E to generate the LEGO-style image. Finally, the resulting image URL is sent back to the user through LINE's reply API.

## Output Details
The workflow sends the generated LEGO-style image back to the LINE user who initiated the request.

## Tags
LINE bot, DALL-E, OpenAI, image transformation, LEGO style, webhook, automation, n8n, production-ready
