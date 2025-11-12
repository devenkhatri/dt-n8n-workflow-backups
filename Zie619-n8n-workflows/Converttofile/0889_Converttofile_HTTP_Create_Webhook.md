# Workflow Analysis for Product Photography Automation with AI

## Description
This workflow automates the creation of professional product photography using AI. It reads product image URLs from a Google Sheet, downloads and analyzes each image to understand what the product is, generates a tailored AI prompt for realistic product photography featuring a human model, sends the original image and prompt to an AI image generation service, uploads the resulting high-quality image to Google Drive, and updates the original sheet with the new image link and prompt used.

## Input Details
The workflow is triggered manually and receives product image URLs from a Google Sheet named 'Image Generation'.

## Process Summary
First, the workflow reads image URLs from a Google Sheet and downloads each image. It then uses an AI model to analyze each image and generate a short description. Based on that description, it creates a detailed prompt for generating professional product photography that includes a human model. The original image and generated prompt are sent to an AI image generation API. The resulting image is converted from base64 to a file, uploaded to Google Drive, and the Google Sheet is updated with the new image URL and the prompt used.

## Output Details
The workflow produces AI-generated professional product photos uploaded to Google Drive and updates the source Google Sheet with the new image links and the prompts used for generation.

## Tags
AI image generation, product photography, Google Sheets, Google Drive, OpenAI, image analysis, automation, e-commerce
