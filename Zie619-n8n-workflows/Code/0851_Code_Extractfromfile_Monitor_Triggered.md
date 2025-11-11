# Workflow Analysis for Automated Purchase Order Processing from Outlook Emails

## Description
This workflow automatically processes purchase orders received as Excel (.xlsx) file attachments in Outlook emails. It converts the Excel file to a markdown table for AI processing, extracts structured purchase order details using an LLM, validates the data for common errors, and sends automated replies to the sender—either confirming acceptance or listing validation issues.

## Input Details
The workflow is triggered by incoming emails in a Microsoft Outlook inbox that contain .xlsx file attachments, which are expected to be purchase order forms.

## Process Summary
The workflow starts by monitoring a shared Outlook inbox for new emails with attachments. It checks if the email intends to submit a purchase order and whether the attachment is an Excel file. If valid, it converts the Excel sheet to a markdown table, then uses an AI model to extract structured purchase order data like vendor info, line items, and totals. It runs validation checks on the extracted data (e.g., PO number presence, date validity, item list, and math accuracy), fixes Excel date formatting if needed, and sends an automated reply—either accepting the PO or listing errors. Validated purchase order data is then ready for integration with internal systems.

## Output Details
The workflow sends automated email replies to the sender (acceptance or rejection with reasons) and outputs structured purchase order data for downstream processing in internal systems like ERPs.

## Tags
purchase order automation, Excel to markdown, AI data extraction, Outlook integration, document processing, LLM workflow, data validation, n8n automation
