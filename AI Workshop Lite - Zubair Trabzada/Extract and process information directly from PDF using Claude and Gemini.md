# Workflow Analysis for PDF Data Extraction Comparison with Claude and Gemini

## Description
This workflow facilitates the comparison of Claude 3.5 Sonnet and Gemini 2.0 Flash models for extracting specific data from a PDF document. It allows users to observe and evaluate the performance, latency, and cost of each AI model for document processing tasks.

## Input Details
The workflow is manually triggered and receives a user-defined prompt along with a specified PDF file downloaded from Google Drive.

## Process Summary
First, the workflow defines a prompt for data extraction and downloads a specified PDF file from Google Drive. The downloaded PDF is then converted into a base64 encoded string. This base64 PDF data and the defined prompt are simultaneously sent to both the Claude 3.5 Sonnet API and the Gemini 2.0 Flash API. Both AI models process the PDF content according to the provided prompt to extract the requested information.

## Output Details
The workflow produces responses from both the Anthropic Claude 3.5 Sonnet and Google Gemini 2.0 Flash APIs, containing the extracted data based on the provided prompt.
