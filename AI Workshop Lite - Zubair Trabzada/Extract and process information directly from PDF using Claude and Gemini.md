# Workflow Analysis for Extract data from PDF with Claude 3.5 Sonnet or Gemini 2.0 Flash

## Description
This workflow extracts structured data from a PDF file using either Google's Gemini 2.0 Flash or Anthropic's Claude 3.5 Sonnet AI models. It enables comparison between the two models in terms of accuracy, speed, and cost for document processing tasks.

## Input Details
The workflow is triggered manually and uses a predefined PDF file from Google Drive along with a user-defined prompt specifying what data to extract.

## Process Summary
The workflow starts by defining a prompt that instructs the AI models on what data to extract from the PDF. It then downloads the specified PDF file from Google Drive and converts it to a base64-encoded string. This encoded file and the prompt are simultaneously sent to both Claude 3.5 Sonnet and Gemini 2.0 Flash APIs. Each AI model processes the PDF and returns the extracted information based on the prompt. The results from both models can be compared for performance and accuracy.

## Output Details
The workflow returns the extracted data from both AI models (Claude and Gemini) as API responses, which can be viewed in the n8n editor or further processed.

## Tags
PDF extraction, AI, Claude, Gemini, document processing, LLM, Google Drive, base64, data extraction, comparison
