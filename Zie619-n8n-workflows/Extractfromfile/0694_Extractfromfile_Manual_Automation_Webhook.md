# Workflow Analysis for Extract Data from PDF with Claude 3.5 Sonnet or Gemini 2.0 Flash

## Description
This workflow compares two AI models—Claude 3.5 Sonnet and Gemini 2.0 Flash—by sending them the same PDF document and prompt to extract structured data (like VAT numbers). It demonstrates how to process PDFs directly with AI APIs without needing separate OCR steps.

## Input Details
The workflow is manually triggered and uses a predefined Google Drive file ID and a user-defined prompt to extract data from a PDF.

## Process Summary
The workflow starts by defining a text prompt for data extraction. It then downloads a specified PDF file from Google Drive and converts it into a base64-encoded string. This encoded PDF and the prompt are sent simultaneously to both Claude 3.5 Sonnet and Gemini 2.0 Flash via their respective APIs. Each AI model processes the PDF and returns structured data based on the prompt. The results from both models can be compared for accuracy, speed, and cost.

## Output Details
The workflow outputs the extracted data from both AI models, which can be viewed in the execution logs or further processed in downstream applications.

## Tags
PDF processing, AI comparison, Claude 3.5 Sonnet, Gemini 2.0 Flash, Google Drive, data extraction, manual trigger, n8n
