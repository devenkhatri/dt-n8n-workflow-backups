# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow automates cloning competitor Facebook ads by analyzing their ad creatives and generating new ads that feature the user's product while preserving the original ad’s style and layout.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow starts by scraping Facebook ads from the provided URL using an Apify actor. It then iterates through each ad, downloads the ad image, and uploads it as a reference to Google Drive. Both the user's product image and the competitor's ad image are converted to base64 format. A detailed AI prompt is constructed to guide Google Gemini in generating a new ad that replaces the competitor's product with the user's while preserving the original style. The AI first creates an editing prompt and then uses it to produce the final cloned ad image, which is saved to Google Drive if valid.

## Output Details
The workflow produces cloned ad images featuring the user's product in the style of competitor ads and uploads them to a specified Google Drive folder.

## Tags
facebook ads, ad cloning, image generation, AI-powered, Google Drive, competitor analysis, marketing automation
