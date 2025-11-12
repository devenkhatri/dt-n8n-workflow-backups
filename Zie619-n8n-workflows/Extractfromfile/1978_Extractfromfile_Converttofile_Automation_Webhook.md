# Workflow Analysis for Extract text from PDF and image using Vertex AI (Gemini) into CSV

## Description
This workflow automatically extracts transaction data from PDFs and images (like bank statements or screenshots), uses AI to interpret and categorize the transactions, and saves the results as a CSV file in Google Drive.

## Input Details
The workflow is triggered when a new file (PDF or image) is added to a specific Google Drive folder.

## Process Summary
The workflow monitors a Google Drive folder for new files. When a PDF or image is uploaded, it downloads the file and routes it based on its type. PDFs are processed to extract raw text, while images are sent to Google's Vertex AI (Gemini) for OCR and text extraction. Both data streams are then sent to an AI service (via OpenRouter) with instructions to format the transactions into CSV with a 'category' column. The resulting CSV data is converted into a file and uploaded to a designated Google Drive folder.

## Output Details
The workflow outputs a CSV file containing parsed and categorized transaction data, which is saved to a specific folder in Google Drive.

## Tags
PDF extraction, OCR, Vertex AI, Gemini, Google Drive, AI automation, CSV export, bank statement parsing, n8n, production-ready
