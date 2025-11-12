# Workflow Analysis for Bank Statement to Markdown Converter using Vision AI

## Description
This workflow converts bank statement PDFs—whether digital or scanned—into structured markdown using vision AI. It splits the PDF into individual page images, processes each with a multimodal language model to extract text and tables faithfully, and then compiles the results for further data extraction, such as identifying deposit transactions.

## Input Details
The workflow is triggered manually and begins by downloading a bank statement PDF from Google Drive.

## Process Summary
The workflow first downloads a bank statement PDF from Google Drive. It then sends the PDF to an external service (via HTTP request) to split it into individual page images, which are returned as a ZIP file. The ZIP is extracted, and the images are converted into a list format. Each image is resized to optimize processing speed and then sent one-by-one to Google's Gemini 1.5 Pro vision model with instructions to transcribe the content into markdown, preserving tables and layout. Finally, all transcribed pages are combined into a single markdown document.

## Output Details
The workflow outputs a consolidated markdown representation of the entire bank statement, which can be used downstream for structured data extraction like identifying deposit rows.

## Tags
PDF processing, Vision AI, Google Gemini, Bank Statement, OCR alternative, Markdown conversion, n8n, automation, document parsing, LLM
