# Workflow Analysis for Googlesheetstool Workflow

## Description
This workflow provides a CV parsing service where users upload PDF resumes, and the system extracts structured data using an AI language model. It logs token usage and costs per client into a Google Sheet and automatically generates monthly invoices based on the logged usage.

## Input Details
The workflow is triggered by a form submission where a user uploads a PDF CV and acknowledges service usage; it receives the uploaded file and client acknowledgment.

## Process Summary
First, the uploaded PDF is parsed to extract raw text. Then, client identifiers like workflow ID, execution ID, and a hardcoded client ID are added to the data. A custom LLM subnode processes the text to extract structured resume data in JSON format, while also capturing token usage and cost via a callback function. This usage data is appended to a Google Sheet for tracking. Separately, at the end of each month, the workflow retrieves all logs for a specific client from the sheet, filters them for the current month, calculates total tokens and costs, and emails an invoice to the client.

## Output Details
The workflow outputs structured JSON data of the parsed CV to the user via a form response, logs detailed token usage and cost data to a Google Sheet, and sends a monthly invoice email with usage totals to a client.

## Tags
automation, n8n, production-ready, excellent, optimized, AI, LLM, token tracking, billing, Google Sheets, CV parsing, invoice generation, self-hosted
