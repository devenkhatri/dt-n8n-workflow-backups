# Workflow Analysis for Image Analysis with AWS Rekognition and Google Sheets Integration

## Description
This workflow automates the process of analyzing images for labels and text using AWS Rekognition and then records the results in a Google Sheet. It also includes an option to search for images via Google Custom Search.

## Input Details
The workflow is triggered manually and takes no initial input data.

## Process Summary
The workflow starts by optionally searching for images using Google Custom Search if a query is provided. It then iterates through the found images or a predefined image URL. For each image, it downloads the image data and sends it to AWS Rekognition for label and text detection. Finally, it constructs a row of data containing the image URL, detected labels, and detected text, and appends this row to a specified Google Sheet.

## Output Details
The workflow outputs image analysis results (labels and text) to a Google Sheet.
