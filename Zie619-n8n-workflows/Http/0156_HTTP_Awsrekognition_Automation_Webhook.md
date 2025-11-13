# Workflow Analysis for Production Workflow

## Description
This workflow fetches an image from an external source, analyzes it using AWS Rekognition to detect visual labels, and logs the image name, link, and detected labels into a Google Sheet.

## Input Details
The workflow is manually triggered and does not receive external input data at initiation.

## Process Summary
The workflow starts with a manual trigger. It makes an HTTP request to a configurable base URL to fetch image data. The retrieved image is sent to AWS Rekognition to detect visual labels. A Set node formats the image title, link, and detected labels into a structured format. Finally, this data is appended to a specified Google Sheet.

## Output Details
The workflow appends a row containing the image name, image link, and detected labels to a Google Sheet.

## Tags
automation, n8n, production-ready, image analysis, AWS Rekognition, Google Sheets, manual trigger
