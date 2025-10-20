# Workflow Analysis for Bill Bot Workflow

## Description
This workflow automates the process of extracting information from bills and generating responses based on the extracted data.

## Input Details
The workflow is triggered by an HTTP request received via a webhook.

## Process Summary
First, the workflow extracts text from an image URL provided in the webhook data using an OCR service. Then, it uses a large language model to comprehend the extracted text and determine if it represents an invoice or a bill. If it is an invoice or bill, the workflow extracts specific details such as the company name, total amount, and due date. Finally, it generates a response based on whether an invoice/bill was identified and the details extracted.

## Output Details
The workflow outputs a JSON response containing an acknowledgment, a generated answer, and the extracted company name, total amount, and due date if applicable.
