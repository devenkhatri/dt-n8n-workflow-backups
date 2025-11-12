# Workflow Analysis for AI Image Captioning with Google Gemini

## Description
This workflow automatically generates a descriptive and punny caption for an image using Google's Gemini multimodal AI model, then overlays the caption directly onto the image for use in publications, social media, or watermarking.

## Input Details
The workflow is manually triggered and fetches an image from a predefined URL using an HTTP request node.

## Process Summary
The workflow begins by downloading an image from a given URL. It then retrieves image metadata and resizes the image to 512x512 pixels for compatibility with the AI model. Next, it sends the resized image to Google Gemini with instructions to generate a caption containing a title and descriptive text. The AI’s structured output is merged with the original image data. A code node calculates optimal text positioning at the bottom of the image based on dimensions and caption length. Finally, the caption is overlaid onto the image using the Edit Image node with a semi-transparent background and white text.

## Output Details
The workflow produces a new image with the AI-generated caption overlaid at the bottom and can be used for publishing, sharing, or further processing.

## Tags
AI image captioning, Google Gemini, image editing, multimodal AI, n8n automation, social media automation, image overlay, content generation
