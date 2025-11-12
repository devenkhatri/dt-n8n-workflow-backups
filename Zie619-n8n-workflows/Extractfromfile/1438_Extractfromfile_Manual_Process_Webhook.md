# Workflow Analysis for Manualtrigger Workflow

## Description
This workflow compares the performance of Claude 3.5 Sonnet and Gemini 2.0 Flash in extracting structured data (like VAT numbers) directly from a PDF file without requiring a separate OCR step. It downloads a PDF from Google Drive, converts it to base64, and sends it to both AI models using custom prompts, enabling side-by-side evaluation of accuracy, speed, and cost.

## Input Details
The workflow is triggered manually and uses a predefined Google Drive file ID and a customizable prompt defined in the 'Define Prompt' node.

## Process Summary
The workflow starts with a manual trigger, then defines a prompt for data extraction. It downloads a PDF file from Google Drive and converts it to a base64-encoded string. This encoded file and the prompt are sent in parallel to both Claude 3.5 Sonnet and Gemini 2.0 Flash via HTTP requests. Each AI model processes the PDF and returns the extracted data based on the prompt.

## Output Details
The workflow produces structured data responses from both Claude and Gemini APIs, which can be used for comparison or further processing.

## Tags
PDF processing, AI comparison, Claude 3.5 Sonnet, Gemini 2.0 Flash, Google Drive, manual trigger, data extraction, base64 encoding, LLM integration, invoice processing
