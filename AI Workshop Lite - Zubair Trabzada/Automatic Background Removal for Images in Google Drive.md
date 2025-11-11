# Workflow Analysis for Remove Advanced Background from Google Drive Images

## Description
This workflow automatically removes the background from new images uploaded to a specified Google Drive folder, applies padding and optional resizing, and saves the processed image with a transparent or colored background back to another Google Drive folder.

## Input Details
The workflow is triggered when new image files are added to a configured Google Drive folder.

## Process Summary
When a new image is detected, it is downloaded from Google Drive. The workflow then reads the image's dimensions and combines them with user-defined settings like background color, padding, and output size preferences. Using the Photoroom API, the background is removed either maintaining the original size or resizing to a fixed dimension. The resulting image is uploaded back to a specified Google Drive folder with a renamed filename indicating the background has been removed.

## Output Details
The workflow outputs background-removed images as PNG files uploaded to a designated Google Drive folder.

## Tags
google drive, image processing, background removal, photoroom api, automation, image editing
