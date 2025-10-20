# Workflow Analysis for Telegram Receipt Textract Workflow

## Description
This workflow automates the process of extracting text from images of receipts received via Telegram and storing the extracted information. This helps businesses digitize their receipts and automate data entry, thereby enhancing efficiency and reducing manual errors.

## Input Details
This workflow is triggered manually and receives image data from a Telegram message.

## Process Summary
This workflow starts by receiving an image file from a Telegram chat. It then uses the n8n Telegram node to retrieve the image. Following this, the image is sent to Amazon Textract for optical character recognition (OCR) to extract text content, which is then stored in the workflow for subsequent use.

## Output Details
The workflow outputs the extracted text from the receipt image.
