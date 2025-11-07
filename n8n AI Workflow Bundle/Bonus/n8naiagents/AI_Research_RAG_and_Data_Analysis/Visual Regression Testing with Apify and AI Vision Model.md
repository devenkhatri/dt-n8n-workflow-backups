# Workflow Analysis for AI-Powered Visual Regression Testing with Google Gemini

## Description
This workflow automates visual regression testing for websites using an AI vision model. It manages website screenshots in Google Sheets and Google Drive, taking new screenshots and comparing them against established base images using Google Gemini. Any detected visual changes are reported as issues in Linear.

## Input Details
The workflow is triggered either manually or on a schedule, reading a list of webpages and their base image references from a Google Sheet.

## Process Summary
1. The workflow retrieves a list of webpages and their base image references from a Google Sheet.
2. For each webpage, it downloads the existing base screenshot from Google Drive and generates a new screenshot using Apify.
3. These two screenshots (base and current) are then sent to a Google Gemini Vision Model via a Langchain LLM Chain.
4. The Gemini model identifies visual differences in text, images, colors, positions, and layouts between the two screenshots, returning a structured JSON output of detected changes.
5. Items with identified changes are filtered, aggregated, and formatted into a markdown report.

## Output Details
The workflow creates new issues in Linear, detailing the detected visual regression changes for each webpage.
