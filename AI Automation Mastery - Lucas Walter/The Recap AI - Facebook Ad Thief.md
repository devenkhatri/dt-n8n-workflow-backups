# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow helps users clone and adapt competitor Facebook ads for their own product by analyzing competitor ad imagery and generating new ads featuring the user's product with matching style and layout.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and an uploaded product image.

## Process Summary
First, the user's product image is converted to base64. Then, the provided Facebook Ad Library URL is scraped to collect competitor ad data. Each ad is processed individually: the ad image is downloaded, converted to base64, and saved to Google Drive as a reference. A detailed prompt is constructed instructing an AI to generate a new ad that mimics the competitor's style but features the user's product (ThriveMix) instead of the competitor's (AG1), including replacing any partial or full branding. The prompt and both images are sent to Google's Gemini AI to generate a new ad image. If the result is not flagged as prohibited content, the generated image is saved to Google Drive with a sequential name.

## Output Details
The workflow produces AI-generated ad images based on competitor ads but featuring the user's product, and saves them to a specified Google Drive folder.

## Tags
facebook ads, ad cloning, image generation, AI, Google Drive, competitor analysis, marketing automation
