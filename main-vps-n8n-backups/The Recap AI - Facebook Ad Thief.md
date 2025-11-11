# Workflow Analysis for The Recap AI - Facebook Ad Thief

## Description
This workflow helps users clone and adapt Facebook ads from competitors by analyzing a competitor's ad image and the user's own product image, then generating a new ad image that mimics the competitor's style but features the user's product branding instead.

## Input Details
The workflow is triggered by a user submitting a form with a Facebook Ad Library URL and uploading their product image.

## Process Summary
The workflow starts by scraping ads from the provided Facebook Ad Library URL. It processes each ad by downloading the ad image and converting both the competitor's ad image and the user's product image to base64 format. It then uses Google's Gemini AI models to first generate a detailed prompt describing how to adapt the competitor's ad to feature the user's product, and then uses that prompt to generate a new ad image. The workflow checks if the generated image contains prohibited content, and if not, uploads the final cloned ad image to a specified Google Drive folder.

## Output Details
The workflow uploads the newly generated ad image (with the user's product) to a Google Drive folder and skips upload if the AI flags the content as prohibited.

## Tags
facebook ads, image generation, AI, ad cloning, Google Drive, Gemini AI, competitor analysis
