# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow allows users to clone and spin Facebook ads for their product by providing a product image and a Facebook Ad Library URL. It leverages AI to generate new ad creatives based on competitor ads, adapting them to feature the user's product.

## Input Details
The workflow is triggered by a form submission, requiring a Facebook Ad Library URL and a product image file.

## Process Summary
The workflow initiates by converting the uploaded product image to a base64 string. Subsequently, it scrapes ads from the provided Facebook Ad Library URL. For each scraped ad, the original image is downloaded, converted to base64, and uploaded to Google Drive as a reference. A detailed AI prompt is then constructed using both the product image and the competitor ad image. This prompt is sent to a Gemini AI model to generate new ad creatives, which are then checked for prohibited content, processed, and finally uploaded as new ad images to Google Drive.

## Output Details
The workflow produces new ad creatives, which are uploaded as images to a designated Google Drive folder. Additionally, the original reference ad images are also stored in Google Drive.
