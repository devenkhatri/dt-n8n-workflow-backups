# Workflow Analysis for Gemini 2.0 Prompt-Based Object Detection with Bounding Box Visualization

## Description
This workflow demonstrates how to use Google's Gemini 2.0 API to detect specific objects in an image based on a text prompt (e.g., 'all rabbits'), then scales the detected bounding box coordinates to match the original image dimensions and overlays them visually.

## Input Details
The workflow is triggered manually and fetches a test image from a URL defined in the environment variable WEBHOOK_URL.

## Process Summary
The workflow begins by downloading a test image and extracting its width and height. It then sends the image along with a prompt to Gemini 2.0 API to detect specified objects and return bounding box coordinates in a normalized 0–1000 range. These coordinates are scaled to match the original image dimensions using a code node. Finally, the workflow draws the scaled bounding boxes onto the original image using the Edit Image node.

## Output Details
The workflow produces an annotated image with bounding boxes drawn around detected objects (e.g., rabbits) and displays it in a sticky note for visual verification.

## Tags
object detection, Gemini AI, image processing, bounding box, prompt-based detection, n8n, automation, computer vision
