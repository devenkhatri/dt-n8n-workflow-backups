# Workflow Analysis for Production Workflow

## Description
This workflow retrieves an image from a provided URL, extracts text from the image using AWS Rekognition, processes the extracted text to lowercase, and appends the image name, image URL, and processed text to a Google Sheet.

## Input Details
The workflow is manually triggered and uses an environment variable 'BASE_URL' to fetch an image file via HTTP request.

## Process Summary
The workflow starts by manually triggering an HTTP request to fetch an image from a predefined URL. It then sends the image to AWS Rekognition to detect and extract text. The extracted text from the first few detections is concatenated into a single string. A 'Set' node formats this data along with the image name and URL. A Function node converts the extracted text to lowercase. Finally, the processed data is appended to a specified Google Sheet.

## Output Details
The workflow appends a row to a Google Sheet containing the image file name, image URL, and the lowercase version of the extracted text.

## Tags
OCR, image processing, AWS Rekognition, Google Sheets, manual trigger, text extraction, automation
