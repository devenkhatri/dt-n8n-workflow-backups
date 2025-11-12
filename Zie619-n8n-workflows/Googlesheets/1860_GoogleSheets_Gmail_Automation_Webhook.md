# Workflow Analysis for WordPress Contact Form (CF7) Responses and Classification

## Description
This workflow automatically processes incoming contact form submissions from a WordPress site, classifies the message type (e.g., product inquiry or order question), generates a tailored draft response using AI, saves the data to Google Sheets, and prepares the draft email for review before sending.

## Input Details
The workflow is triggered by a POST webhook from a WordPress Contact Form 7 submission, receiving fields like first name, last name, email, phone, and message.

## Process Summary
The workflow starts by receiving form data via a webhook and extracting key fields. It then classifies the message into predefined categories like 'Product Info' or 'Order Info' using an AI text classifier. Based on the classification, it routes the message to a specialized AI agent that drafts a personalized email response with an appropriate subject and body. The draft response, along with the original message and contact info, is saved to a Google Sheet for record-keeping. Finally, the workflow creates a Gmail draft addressed to the customer, ready for human review and sending.

## Output Details
The workflow produces categorized customer contact records in a Google Sheet and creates categorized draft emails in Gmail for internal review and sending.

## Tags
wordpress, contact form, CF7, AI classification, email automation, Google Sheets, Gmail draft, customer support, workflow automation, n8n
