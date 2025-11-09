# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow automatically creates new ad creatives by analyzing competitor Facebook ads and using AI to rebrand them with the user's product, enabling rapid ad creation inspired by successful competitor campaigns.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a user-provided product image file.

## Process Summary
The workflow converts the user's product image to base64 format, then scrapes competitor ads from the provided Facebook Ad Library URL using an Apify actor. For each competitor ad, it downloads the image, converts it to base64, and saves the original to Google Drive. It constructs a custom AI prompt to replace competitor branding with the user's product (ThriveMix) and uses Google's Gemini API to generate an image-editing prompt and produce a rebranded ad image. Finally, it checks the generated image for content policy violations before proceeding.

## Output Details
The workflow uploads approved, rebranded ad images featuring the user's product to a designated Google Drive folder.

## Tags
facebook ads, ad generation, image editing, AI, Google Drive, competitor analysis, ad cloning, Gemini API, Apify
