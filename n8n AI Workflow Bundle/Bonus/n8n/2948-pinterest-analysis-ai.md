# Workflow Analysis for Pinterest Image Analysis with AI

## Description
This workflow analyzes images from Pinterest pins using artificial intelligence to extract meaningful information and store it in a Google Sheet. It helps businesses understand visual content trends and automate data entry for Pinterest analytics.

## Input Details
The workflow is manually triggered and receives a list of Pinterest pin URLs as input.

## Process Summary
The workflow starts by extracting image URLs from the provided Pinterest pin URLs. It then processes each image by making an API call to a vision AI service to describe the image content. The AI-generated descriptions are then used to further classify the images using another AI service to determine the dominant color and categorize the image topic. Finally, all the extracted information, including pin URL, image URL, AI description, dominant color, and image topic, is appended as a new row to a specified Google Sheet.

## Output Details
The workflow outputs a new row in a Google Sheet containing the Pinterest pin URL, image URL, AI description, dominant color, and image topic.
