# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow automatically generates new Facebook ad creatives that mimic competitor ad styles by replacing competitor branding with the user's own product image using AI.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and an uploaded product image file.

## Process Summary
The workflow converts the uploaded product image to base64 format and scrapes Facebook ads from the provided URL using an Apify actor. For each scraped ad, it downloads the ad image, converts it to base64, and saves it to Google Drive as a reference. It then constructs a detailed AI prompt to clone the competitor ad while substituting all branding with the user's product (ThriveMix). Both images and the prompt are sent to Google's Gemini AI, and if the response is not blocked for prohibited content, the generated ad image is extracted. Finally, the AI-generated ad image is uploaded to a specified Google Drive folder.

## Output Details
The workflow produces new AI-generated ad images that replicate competitor ad styles featuring the user's product and saves them to a designated Google Drive folder.

## Tags
facebook ads, ad generation, image cloning, AI image generation, Google Drive, competitor analysis, marketing automation
