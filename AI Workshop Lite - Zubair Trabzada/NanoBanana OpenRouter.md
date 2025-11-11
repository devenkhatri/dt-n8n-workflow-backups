# Workflow Analysis for NanoBanana OpenRouter

## Description
This workflow generates UGC-style ads by taking a user-submitted image and description, analyzing the image to understand its content, generating a tailored AI image prompt based on that analysis and the user's input, and then using an external AI model via OpenRouter to produce a new ad-like image that incorporates those details.

## Input Details
The workflow is triggered by a form submission that includes an image file and a text description from the user.

## Process Summary
First, the submitted image is uploaded to Google Drive. Then, an OpenAI model analyzes the image to determine if it shows a product, character, or both, and extracts relevant visual details in YAML format. This analysis, combined with the user's description, is used to generate a structured image prompt following ad-generation guidelines. The prompt and original image are sent to OpenRouter (using Google's Gemini model) to generate a new ad-like image. Finally, the generated image is parsed, formatted, and converted into a downloadable file.

## Output Details
The workflow produces a newly generated UGC-style ad image based on the user's input and returns it as a downloadable file.

## Tags
UGC, image generation, ad creation, OpenRouter, Google Drive, OpenAI, form submission, AI image editing
