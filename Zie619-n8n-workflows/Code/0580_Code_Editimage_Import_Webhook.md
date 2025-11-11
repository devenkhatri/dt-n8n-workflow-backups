# Workflow Analysis for Bank Statement to Markdown Converter Using Vision AI

## Description
This workflow converts a bank statement PDF—whether scanned or digital—into structured markdown using vision AI. It processes each page as an image, transcribes it faithfully into markdown (including tables), and then extracts key deposit information using a language model.

## Input Details
The workflow is manually triggered and starts by downloading a bank statement PDF from Google Drive.

## Process Summary
First, the workflow downloads a bank statement PDF from Google Drive. It then sends the PDF to an external service (Stirling PDF) to split it into individual page images, which are returned in a zip file. The zip is extracted, and each image is prepared as a separate item in a list. Images are resized to optimize AI processing speed without losing critical detail. Each image is then sent to Google Gemini, a vision-capable AI model, with instructions to transcribe the content into markdown while preserving tables and structure. The markdown from all pages is aggregated into a single document. Finally, another AI call extracts only the deposit entries from the combined markdown using a defined schema.

## Output Details
The workflow outputs a structured list of deposit transactions extracted from the bank statement, ready for downstream use such as accounting or analytics.

## Tags
PDF processing, OCR, vision AI, bank statement, markdown conversion, Google Gemini, document automation, financial data extraction, n8n, LLM
