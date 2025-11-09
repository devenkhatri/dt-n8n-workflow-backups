# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow automatically creates new Facebook ad creatives by analyzing competitor ads and using AI to replace their branding with the user's own product image, effectively mimicking successful competitor ad styles.

## Input Details
Triggered by a form submission that includes a Facebook Ad Library URL and an uploaded product image file.

## Process Summary
The workflow first converts the user's uploaded product image to base64. It then scrapes competitor ads from the provided Facebook Ad Library URL using an Apify actor. For each scraped ad, it downloads the ad image, converts it to base64, and saves it to Google Drive as a reference. A custom AI prompt is constructed to instruct Gemini AI to clone the competitor ad while replacing all branding with the user's product (ThriveMix). The generated ad image is extracted from Gemini's response if not blocked for prohibited content and uploaded to a specified Google Drive folder.

## Output Details
AI-generated ad images that replicate competitor ad styles featuring the user's product are saved to a designated Google Drive folder.

## Tags
facebook ads, ad generation, image cloning, AI image generation, Google Drive, competitor analysis, marketing automation
