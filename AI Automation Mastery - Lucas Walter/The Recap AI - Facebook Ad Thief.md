# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow enables users to automatically generate new ad creatives that mimic competitor Facebook ads but showcase the user's own product by using AI to analyze, rebrand, and recreate ad images.

## Input Details
The workflow is triggered by a form submission that includes a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow first converts the user-submitted product image to base64. It then scrapes competitor ads from the provided Facebook Ad Library URL using an Apify actor. For each scraped ad, it downloads and converts the ad image to base64, and uploads the original to Google Drive as a reference. A custom AI prompt is constructed to guide the replacement of competitor branding with the user's product branding (ThriveMix), and Google’s Gemini API is used to generate an image-editing prompt and then the final rebranded ad image. The workflow checks for content policy violations before saving approved images to Google Drive.

## Output Details
The workflow generates new, rebranded ad images featuring the user's product and uploads them to a specified Google Drive folder.

## Tags
facebook ads, ad generation, image editing, AI, Google Drive, competitor analysis, ad cloning, Gemini API, Apify
