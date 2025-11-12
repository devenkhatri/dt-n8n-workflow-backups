# Workflow Analysis for Contact Form Text Classifier for eCommerce

## Description
This workflow automatically classifies incoming contact form messages from an eCommerce website into predefined categories like 'Request Quote', 'Product info', 'General problem', or 'Order', then routes each message to the appropriate department via email and logs it in a shared Google Sheet for tracking.

## Input Details
The workflow is triggered when a user submits a contact form containing their name, email, and message.

## Process Summary
When a form is submitted, the workflow uses OpenAI's GPT-4o-mini model to classify the message into one of five categories. Based on the classification, it sends a tailored email to the relevant department (e.g., Quotes, Product, General, Order, or Other) with the contact details and message. Simultaneously, it appends the submission data—including timestamp, name, email, message, and category—to a Google Sheet named 'Classified Contact Form' for record-keeping and analytics.

## Output Details
The workflow sends categorized emails to departmental inboxes and logs all submissions in a Google Sheet for tracking and reporting.

## Tags
eCommerce, contact form, text classification, OpenAI, email automation, Google Sheets, n8n, workflow automation, customer support, message routing
