# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow allows users to upload their product image and a Facebook Ad Library URL to automatically generate new ad creatives that replicate competitors' ad styles while showcasing the user's own product.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and an uploaded product image file.

## Process Summary
The workflow first converts the uploaded product image to base64 format. It then scrapes Facebook ads from the provided URL using an Apify actor and downloads each competitor ad image, converting them to base64 and uploading to Google Drive for reference. A detailed prompt combining the competitor ad style and user's product is constructed and sent to an AI model, which refines the prompt and generates a new ad image. The system checks if the AI response was blocked due to prohibited content. If not blocked, the generated image is saved to Google Drive with a sequential filename.

## Output Details
The workflow produces and saves AI-generated ad images that mimic competitor ads but feature the user's product to a specified Google Drive folder.

## Tags
facebook ads, AI image generation, ad cloning, competitor analysis, Google Drive, Apify, Gemini AI, image editing, marketing automation
