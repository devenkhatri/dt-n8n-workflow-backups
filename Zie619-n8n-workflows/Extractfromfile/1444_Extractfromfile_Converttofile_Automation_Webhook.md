# Workflow Analysis for Extract text from PDF and image using Vertex AI (Gemini) into CSV

## Description
This workflow automatically extracts transaction data from uploaded PDFs or images (like bank statements), uses AI to interpret and categorize the content, and saves the results as a structured CSV file in Google Drive.

## Input Details
The workflow is triggered when a new file (PDF or image) is added to a specified Google Drive folder.

## Process Summary
When a file is uploaded to a Google Drive folder, the workflow checks whether it's a PDF or an image. PDFs are downloaded and text is extracted directly, while images are processed using Google's Vertex AI (Gemini) to extract text. Both data streams are then sent to an AI service (via OpenRouter) with instructions to parse the content as financial transactions, add a category column, and return CSV-formatted data. The resulting CSV is saved to a designated Google Drive folder with today's date as the filename.

## Output Details
The workflow produces a CSV file containing parsed and categorized transaction data, which is uploaded to a specified Google Drive folder.

## Tags
PDF processing, image text extraction, Vertex AI, Gemini, CSV export, Google Drive automation, bank statement parsing, AI data extraction, n8n workflow, production-ready
