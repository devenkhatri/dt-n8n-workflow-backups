# Workflow Analysis for Expense Tracker App

## Description
This workflow automatically captures expense receipts submitted via Typeform, extracts key information like amount, merchant, date, and category using AI-powered receipt parsing, and stores the structured data in an Airtable database for tracking and reporting.

## Input Details
The workflow is triggered when a user submits a receipt through a Typeform form, which includes an uploaded receipt image.

## Process Summary
First, the workflow receives a receipt submission via a Typeform webhook. It then downloads the receipt image using an HTTP request. Next, it uses Mindee’s receipt parsing API to extract structured data such as total amount, merchant name, date, time, and category. The extracted data is reformatted and filtered using a Set node to include only relevant fields. Finally, the cleaned expense data is appended to an Airtable 'Expenses' table.

## Output Details
The workflow stores the parsed expense details (amount, merchant, date, time, receipt URL, and category) as a new record in an Airtable base.

## Tags
expense tracking, receipt parsing, Typeform, Mindee, Airtable, automation, finance, n8n
