# Workflow Analysis for Mistral OCR Document and Image Processing Workflow

## Description
This workflow demonstrates three different approaches to extract text from documents and images using Mistral's OCR capabilities: (1) processing publicly hosted files via URLs, (2) securely uploading private files to Mistral Cloud and processing them via signed URLs, and (3) using Mistral's document-aware language models to directly answer questions about the content of uploaded files.

## Input Details
The workflow is triggered manually and processes two predefined files from Google Drive: one PDF document and one image.

## Process Summary
First, the workflow downloads a PDF and an image from Google Drive. It then uploads both files to Mistral Cloud for secure storage and obtains signed URLs. Using these signed URLs, it performs OCR on both files via Mistral's dedicated OCR API. Separately, it also demonstrates direct document understanding by sending questions about publicly accessible file URLs to Mistral's language models (mistral-small for documents, pixtral-large for images).

## Output Details
The workflow returns structured OCR results (in markdown format) and answers to document-related questions from Mistral's APIs, which can be used for further processing or analysis.

## Tags
OCR, Mistral AI, document processing, image processing, Google Drive, file upload, signed URL, text extraction, automation, n8n
