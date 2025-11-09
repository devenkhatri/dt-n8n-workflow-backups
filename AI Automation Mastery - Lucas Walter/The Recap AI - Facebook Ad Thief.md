# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow enables users to upload a product image and provide a Facebook Ad Library URL to automatically generate new ad images that mimic competitor ads but feature the user's product instead.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow converts the uploaded product image to base64, scrapes Facebook ads from the provided URL using an Apify actor, and downloads each competitor ad image. It converts each ad image to base64 and uploads it to Google Drive as a reference. A detailed prompt is constructed and sent to an AI model to first refine the prompt and then generate a new ad image blending the competitor's style with the user's product. The workflow checks if the AI response was blocked due to prohibited content, and if not, saves the generated image to Google Drive with a sequential filename.

## Output Details
The workflow produces AI-generated ad images that mimic competitor ads but feature the user's product, and saves them to a specified Google Drive folder.

## Tags
facebook ads, AI image generation, ad cloning, competitor analysis, Google Drive, Apify, Gemini AI, image editing, marketing automation
