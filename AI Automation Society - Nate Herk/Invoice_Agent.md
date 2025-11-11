# Workflow Analysis for 🤖Invoice Agent

## Description
This workflow automatically processes invoice images sent via Telegram by extracting key details using OCR, saving the invoice to Google Drive, updating a Google Sheets invoice database, and sending a confirmation message with invoice details and links back to the user.

## Input Details
The workflow is triggered when a user sends a document (invoice image) to a Telegram bot.

## Process Summary
The workflow starts by receiving an invoice image via Telegram, then downloads the file. It sends the image to an OCR service to extract text, parses the text to extract structured invoice data (like invoice number, date, amount, etc.), and appends this data to a Google Sheets database. Simultaneously, the original invoice image is saved to a Google Drive folder. Finally, an AI-powered agent generates a user-friendly response summarizing the invoice details, file name, and database link, which is sent back to the user via Telegram.

## Output Details
The workflow updates a Google Sheets invoice database, saves the original invoice to Google Drive, and sends a detailed confirmation message back to the user on Telegram.

## Tags
invoice processing, OCR, Telegram bot, Google Sheets, Google Drive, AI agent, automation
