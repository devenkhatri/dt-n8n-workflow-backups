# Workflow Analysis for Image to License Plate Number Extractor

## Description
This workflow leverages Artificial Intelligence to automatically detect and extract license plate numbers from images uploaded by the user.

## Input Details
The workflow is initiated by a web form submission where a user uploads an image file (JPG or PNG).

## Process Summary
Initially, the workflow configures an AI model (GPT-4o) and a specific prompt designed to extract license plate numbers from images. It then sends the uploaded image along with this prompt to the AI model for processing. The AI analyzes the image based on the prompt to identify and extract the license plate number from the front-most car.

## Output Details
The workflow displays a completion web page to the user, presenting the extracted license plate number.
