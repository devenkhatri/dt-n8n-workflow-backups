# Workflow Analysis for Gemini 2.0 Prompt-Based Object Detection with Bounding Boxes

## Description
This workflow demonstrates how to use Google's Gemini 2.0 API to perform prompt-based object detection on an image, extract bounding box coordinates for specified objects (e.g., rabbits), scale those coordinates to match the original image dimensions, and overlay the bounding boxes onto the image for visualization.

## Input Details
The workflow is triggered manually and fetches a test image from a URL defined in the environment variable WEBHOOK_URL.

## Process Summary
The workflow starts by downloading a test image and extracting its dimensions. It then sends the image to the Gemini 2.0 API with a prompt requesting bounding boxes around specific objects (rabbits). The API returns normalized coordinates, which are then scaled to the original image size using a code node. Finally, the workflow draws the bounding boxes on the original image using the edit image node.

## Output Details
The workflow produces an image with bounding boxes drawn around detected objects and displays it in a sticky note within the n8n editor.

## Tags
object detection, Gemini AI, image processing, bounding boxes, n8n, HTTP request, image editing, manual trigger, AI vision, prompt-based detection
