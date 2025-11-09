# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow enables users to automatically generate new Facebook ad creatives that mimic competitor ad styles by replacing competitor branding with the user's own product image using AI.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and an uploaded product image file.

## Process Summary
The workflow first converts the uploaded product image to base64 format, then scrapes Facebook ads from the provided URL using an Apify actor. For each scraped ad, it downloads the ad image, converts it to base64, and saves it to Google Drive as a reference. It constructs a detailed AI prompt to clone the competitor ad while substituting all branding with the user's product (ThriveMix), then sends both images and the prompt to Google's Gemini AI. If the AI response is not blocked for prohibited content, the generated ad image is extracted and uploaded to a specified Google Drive folder.

## Output Details
The workflow produces new AI-generated ad images that replicate competitor ad styles featuring the user's product and saves them to a designated Google Drive folder.

## Tags
facebook ads, ad generation, image cloning, AI image generation, Google Drive, competitor analysis, marketing automation
