# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow allows users to upload a product image and provide a Facebook Ad Library URL to automatically generate new ad images that mimic competitor ads but feature the user's product instead. It scrapes competitor ads, analyzes their visual style, and uses AI to create new customized ad images with the user's product branding while preserving the original ad's layout and messaging.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file upload.

## Process Summary
The workflow first converts the uploaded product image to base64 format, then scrapes Facebook ads from the provided URL using an Apify actor. It iterates through each scraped ad, downloads the ad image, and uploads it to Google Drive as a reference. The ad image is also converted to base64. A detailed prompt is constructed instructing the AI to replace competitor branding with the user's product while maintaining the ad's style. The workflow uses Google's Gemini API to generate a new ad image based on both the product and reference images. It checks if the generation was blocked due to prohibited content, and if not, uploads the final generated image to a specified Google Drive folder.

## Output Details
The workflow uploads both reference competitor ad images and newly generated ad images featuring the user's product to designated Google Drive folders.

## Tags
facebook ads, image generation, competitor analysis, google drive, gemini ai, ad creation, image editing, apify scraper
