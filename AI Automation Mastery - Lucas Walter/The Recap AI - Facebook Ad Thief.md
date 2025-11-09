# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow enables marketers to automatically generate new ad creatives that mimic the style of competitors’ Facebook ads while featuring their own product image.

## Input Details
The workflow is triggered by a form submission that includes a Facebook Ad Library URL and an uploaded product image file.

## Process Summary
The workflow converts the uploaded product image to base64, scrapes competitor ads from the provided Facebook Ad Library URL using Apify, and downloads each ad image for reference. These competitor images are converted to base64 and saved to Google Drive. A prompt combining the competitor ad style and the user's product is sent to an AI model, which refines it and generates a new ad image. The system validates that the AI response isn’t blocked due to policy violations. If valid, the generated image is saved to a Google Drive folder with a sequential filename.

## Output Details
The workflow saves AI-generated ad images that replicate competitor styles but feature the user’s product to a designated Google Drive folder.

## Tags
facebook ads, AI image generation, ad cloning, competitor analysis, Google Drive, Apify, Gemini AI, image editing, marketing automation
