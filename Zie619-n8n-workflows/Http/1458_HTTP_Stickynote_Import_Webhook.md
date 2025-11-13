# Workflow Analysis for Optimise images uploaded to GDrive

## Description
This automated workflow optimizes images uploaded to Google Drive. It automatically sends images added to a specific Google Drive folder to tinypng.com for size optimization and then saves the optimized versions back to a chosen Google Drive location.

## Input Details
The workflow triggers when a new file (image) is created in a specific Google Drive folder, receiving the details of the newly created file.

## Process Summary
First, the workflow is triggered upon the creation of a new image file in a designated Google Drive folder. Second, it downloads this newly uploaded image from Google Drive. Third, the downloaded image is sent to the TinyPNG API for optimization. Fourth, the workflow retrieves the optimized image from TinyPNG. Finally, the optimized image is uploaded and saved into a specified Google Drive folder.

## Output Details
The workflow produces optimized image files that are saved back into a designated Google Drive folder.

## Tags
automation, n8n, production-ready, excellent, optimized
