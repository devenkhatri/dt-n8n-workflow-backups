# Workflow Analysis for Combine Images Nanobanana

## Description
This workflow combines multiple product images horizontally and exports the combined image to a specified folder on Google Drive and optionally uploads to Shopify.

## Input Details
This workflow is triggered manually and requires external image URLs and a Google Drive folder ID as input.

## Process Summary
The workflow starts by retrieving image URLs from input data. It then downloads these images, scales them to a uniform height while maintaining aspect ratio, and combines them horizontally into a single image. Finally, the combined image is uploaded to Google Drive. Optionally, the workflow can also upload the image to Shopify if configured.

## Output Details
The workflow outputs a combined image file to a specified Google Drive folder and can optionally upload it to Shopify.
