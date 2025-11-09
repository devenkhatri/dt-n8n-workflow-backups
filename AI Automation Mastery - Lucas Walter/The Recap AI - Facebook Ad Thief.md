# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow allows users to submit a Facebook Ad Library URL and a product image to automatically generate new ad creatives that mimic the style of competitor ads but feature the user's product instead. It uses AI to analyze competitor ads, replace competitor branding with the user's product branding, and generate new ad images that are then saved to Google Drive.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow starts by converting the uploaded product image to base64 format. It then scrapes ads from the provided Facebook Ad Library URL using an Apify actor. For each scraped ad, it downloads the ad image, converts it to base64, and uploads the original ad image as a reference to Google Drive. A detailed prompt is constructed to instruct an AI model on how to replace competitor branding with the user's product (ThriveMix). The workflow uses Google's Gemini API to first generate an image editing prompt and then to generate the new ad image based on that prompt. It checks if the generated content was blocked for policy reasons, and if not, saves the new ad image to a specified Google Drive folder.

## Output Details
The workflow produces new ad images that mimic competitor ads but feature the user's product, and uploads them to a designated Google Drive folder.

## Tags
facebook ads, ad generation, image editing, AI, Google Drive, competitor analysis, ad cloning, Gemini API, Apify
