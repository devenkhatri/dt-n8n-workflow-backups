# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow helps users clone and adapt competitor Facebook ads by using their product image and a competitor's ad URL. It scrapes competitor ads, analyzes them alongside the user's product image using AI, and generates new ad images that mimic the competitor's style while featuring the user's product and branding.

## Input Details
The workflow is triggered by a form submission containing a Facebook Ad Library URL and a product image file upload.

## Process Summary
The workflow starts by scraping Facebook ads from the provided URL using an Apify actor. It then iterates through each ad, downloads the ad image, and uploads it to Google Drive as a reference. Both the user's product image and the competitor's ad image are converted to base64. A detailed prompt is constructed to instruct an AI model (Google Gemini) to generate a new ad image that replicates the competitor's style but features the user's product (ThriveMix) instead of the competitor's (AG1). The AI generates the new ad image, checks if the content was prohibited, and if not, saves the resulting image to Google Drive.

## Output Details
The workflow produces and uploads new ad images to a specified Google Drive folder, with each image cloned from a competitor ad but featuring the user's product and branding.
