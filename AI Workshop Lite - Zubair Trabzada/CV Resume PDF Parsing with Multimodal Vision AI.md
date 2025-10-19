# Workflow Analysis for CV Resume PDF Parsing with Multimodal Vision AI

## Description
This workflow automates the extraction and parsing of CV/resume data from PDF files using AI and then stores the structured information in a Google Sheet and a PDF storage provider.

## Input Details
The workflow is triggered manually and receives PDF data for CV/resume processing.

## Process Summary
The workflow begins by receiving a base64 encoded PDF file. It then decodes the base64 PDF and saves it as a binary file. Next, it uploads this binary file to a cloud storage (Cloudinary) and extracts text from the PDF using a PDF text extractor. Finally, it uses an AI model to process the extracted text and image, and stores the extracted information in a Google Sheet and a PDF storage service.

## Output Details
The workflow outputs structured CV/resume data to a Google Sheet and uploads the processed PDF to a PDF storage service.
