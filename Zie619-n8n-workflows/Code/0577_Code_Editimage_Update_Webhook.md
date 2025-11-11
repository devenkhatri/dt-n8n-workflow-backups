# Workflow Analysis for Image Captioning with Google Gemini and Caption Overlay

## Description
This workflow automatically downloads an image, uses Google Gemini's vision capabilities to generate a creative caption with a title, and overlays that caption onto the image at the bottom with proper formatting and positioning.

## Input Details
The workflow is triggered manually and receives no external input—it fetches a sample image from a predefined URL.

## Process Summary
First, the workflow downloads an image via an HTTP request. It then extracts image metadata and resizes the image to 512x512 for compatibility with the AI model. Next, Google Gemini analyzes the image and generates a structured caption containing a title and descriptive text. The caption is merged with the original image data and sent to a code node that calculates optimal text positioning based on image dimensions. Finally, the workflow draws a semi-transparent background and overlays the caption text at the calculated position on the original image.

## Output Details
The workflow produces a modified image with an AI-generated caption overlaid at the bottom and makes it available as a binary output for download or further use.

## Tags
image processing, AI captioning, Google Gemini, automation, n8n, image overlay, multimodal AI, production-ready
