# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow automates the process of cloning competitor Facebook ads by analyzing their ad creatives and generating new ads featuring the user's own product while preserving the original ad's style and layout.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow starts by scraping Facebook ads from the provided URL using an Apify actor. It then iterates through each ad, downloads the ad image, and uploads it as a reference to Google Drive. Both the user's product image and the competitor's ad image are converted to base64 format. A detailed prompt is constructed to instruct an AI model on how to generate a new ad that replaces the competitor's product with the user's product while maintaining the original ad's style. The AI model (Google Gemini) first generates a detailed editing prompt and then uses it to create the final cloned ad image, which is saved to Google Drive if valid.

## Output Details
The workflow produces cloned ad images featuring the user's product in the style of competitor ads and uploads them to a specified Google Drive folder.

## Tags
facebook ads, ad cloning, image generation, AI-powered, Google Drive, competitor analysis, marketing automation
