# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow allows users to submit a Facebook Ad Library URL and their product image to automatically generate new ad creatives that mimic the style of competitor ads while featuring the user's product instead. It uses AI to analyze competitor ad visuals, replace competitor branding with the user's product, and generate new ad images that are saved to Google Drive.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow starts by converting the uploaded product image to base64 format. It then scrapes Facebook ads from the provided URL using an Apify actor. For each scraped ad, it downloads the ad image, converts it to base64, and uploads it to Google Drive as a reference. A detailed prompt is constructed instructing the AI to clone the competitor ad while replacing all branding with the user's product (ThriveMix). The prompt and both images are sent to Google's Gemini AI to generate a new ad image. The workflow checks if the AI response was blocked due to prohibited content; if not, it extracts and uploads the generated image to a specified Google Drive folder.

## Output Details
The workflow generates new ad images that replicate competitor ad styles with the user's product and saves them to a designated Google Drive folder.

## Tags
facebook ads, ad generation, image cloning, AI image generation, Google Drive, competitor analysis, marketing automation
