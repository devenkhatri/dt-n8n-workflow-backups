# Workflow Analysis for Image to license plate number

## Description
This workflow extracts the license plate number from an uploaded image of a car using AI-powered image analysis. Users submit an image through a web form, and the system returns only the detected license plate characters.

## Input Details
The workflow is triggered by a user uploading a JPG or PNG image via a web form.

## Process Summary
The workflow starts by accepting an image upload through a form trigger. It then sets the AI model to use (GPT-4o) and defines a prompt instructing the model to extract only the license plate number from the front-most car in the image. The configured AI model processes the image and returns the extracted text. Finally, the result is displayed to the user on a completion page showing the extracted license plate number.

## Output Details
The workflow displays the extracted license plate number to the user on a completion web page.

## Tags
automation, n8n, production-ready, excellent, optimized, license plate recognition, image analysis, AI, form submission, LLM
