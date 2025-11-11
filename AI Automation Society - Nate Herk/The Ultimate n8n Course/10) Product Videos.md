# Workflow Analysis for Product Videos

## Description
This workflow automates the creation of professional marketing materials from a product photo, title, and description submitted via a form. It generates an enhanced product image using AI, creates a 3D-like rotating marketing video from that image, and emails both the image and video to the user.

## Input Details
The workflow is triggered by a form submission containing a product photo, title, description, and email address.

## Process Summary
1. When a user submits the form, the product photo is uploaded to Google Drive. 2. An AI agent (using GPT-4.1) generates a detailed prompt to enhance the product photo based on the title and description. 3. The original photo is downloaded and sent to OpenAI's image editing API with the generated prompt to create a professional product image. 4. The enhanced image is converted to a file and uploaded to ImageBB to get a public URL. 5. This URL is sent to Runway ML to generate a 10-second 3D turntable-style marketing video, which is polled until ready, then emailed along with the image link to the user.

## Output Details
The workflow sends an email to the user with links to the AI-enhanced product image and the generated marketing video.

## Tags
marketing automation, AI image generation, video generation, product photography, form processing, Runway ML, OpenAI, Google Drive, email notification
