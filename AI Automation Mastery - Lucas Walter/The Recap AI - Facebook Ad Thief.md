# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow allows users to upload a product image and provide a Facebook Ad Library URL. It then scrapes competitor ads from the URL, uses AI to analyze and clone the ad style, replaces competitor branding with the user's product, and generates new ad images featuring the user's product in the same visual style.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow starts by converting the uploaded product image to base64. It then scrapes Facebook ads from the provided URL using an Apify actor. For each ad, it downloads the ad image, converts it to base64, and uploads it as a reference to Google Drive. A detailed prompt is constructed to instruct an AI model to generate a new ad image that replicates the competitor's style but features the user's product. The AI first generates a refined prompt, then uses that prompt along with both images to create a new ad image. The workflow checks if the AI response was blocked due to prohibited content. If not, the generated image is saved to Google Drive with a sequential name.

## Output Details
The workflow produces AI-generated ad images that mimic competitor ads but feature the user's product, and saves them to a specified Google Drive folder.

## Tags
facebook ads, AI image generation, ad cloning, competitor analysis, Google Drive, Apify, Gemini AI, image editing, marketing automation
