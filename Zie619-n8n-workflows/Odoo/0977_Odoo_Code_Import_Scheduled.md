# Workflow Analysis for Import Odoo Product Images from Google Drive

## Description
Automated workflow: Import Odoo Product Images from Google Drive. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered either manually or on a scheduled interval (every 10 minutes) to process image files from a specific Google Drive folder.

## Process Summary
The workflow is triggered manually or on a schedule. It finds image files (PNG/JPG) in a designated Google Drive folder. For each image, it extracts product model (template or product) and SKU from the filename. Based on the model, it downloads the image, converts it to Base64, and updates the corresponding product or product template in Odoo. Finally, it moves the processed images to a 'done' folder in Google Drive, deletes any old images, and sends a summary notification via Google Chat.

## Output Details
The workflow updates product and product template images in Odoo, archives processed images in Google Drive, and sends a completion notification to Google Chat.

## Tags
automation, n8n, production-ready, excellent, optimized
