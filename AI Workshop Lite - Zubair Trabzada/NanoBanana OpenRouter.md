# Workflow Analysis for UGC Ad Image Generator

## Description
This workflow generates User-Generated Content (UGC) ad images by taking a user's description and an input photo, analyzing the photo, creating an AI image generation prompt, and then using an AI model to produce a new ad image.

## Input Details
The workflow is triggered by a form submission that receives an image description (text) and an image file.

## Process Summary
Upon form submission, the workflow uploads the provided image to Google Drive. It then uses an AI model (ChatGPT-4o) to analyze the uploaded image, extracting details about whether it depicts a product or a character, along with color schemes, styles, and visual descriptions. An "Image Prompt Generator" node, guided by specific ad prompt building instructions, combines the user's description and the image analysis to craft a detailed prompt for an AI image generator. This prompt, along with the original image, is sent to OpenRouter's API (utilizing the Google Gemini-2.5-flash-image-preview model) to generate a new ad image. Finally, the generated image URL from the AI response is processed to extract the image data, which is then converted into a binary file.

## Output Details
The workflow produces a newly generated ad image file based on the user's input and AI processing.
