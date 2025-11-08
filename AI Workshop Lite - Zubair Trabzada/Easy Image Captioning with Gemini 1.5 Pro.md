# Workflow Analysis for AI Image Captioning and Overlay

## Description
This workflow takes an image, uses a Google Gemini AI model to generate a descriptive and punny caption, and then overlays that caption directly onto the image itself.

## Input Details
The workflow is triggered manually and fetches an image from a predefined Pexels URL as its input data.

## Process Summary
First, the workflow downloads an image from a specified URL and extracts its metadata, while also creating a resized version suitable for AI processing. Next, it sends the resized image to a Google Gemini chat model, prompting it to generate a caption title and text in a structured format. After receiving the AI-generated caption, the workflow calculates the optimal position, font size, and text wrapping for the caption based on the original image's dimensions and the caption's length. Finally, it overlays a semi-transparent black rectangle and the generated caption text onto the original image.

## Output Details
The workflow produces a modified image with a dynamically positioned, AI-generated caption title and text overlaid at the bottom.
