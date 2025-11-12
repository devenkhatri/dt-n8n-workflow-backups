# Workflow Analysis for Contact Form Text Classifier for eCommerce

## Description
This workflow automatically classifies incoming customer messages from a contact form into predefined categories like 'Request Quote', 'Product info', 'General problem', or 'Order', then routes each message to the appropriate department via email and logs it in a shared Google Sheet for tracking.

## Input Details
The workflow is triggered by a web form submission containing the user's Name, Email, and Message.

## Process Summary
When a user submits the contact form, the workflow captures the input data. It then uses an AI text classifier (powered by OpenAI's GPT-4o-mini) to categorize the message into one of four predefined types. Based on the classification result, the system sends a formatted email to the corresponding department (e.g., Quotes, Product, Orders, or General). Simultaneously, the message details—including timestamp, name, email, category, and content—are appended to a master Google Sheet for record-keeping and reporting.

## Output Details
The workflow sends a categorized email to the relevant department and logs all submission details in a Google Sheet named 'Classified Contact Form'.

## Tags
eCommerce, contact form, text classification, AI, OpenAI, email automation, Google Sheets, n8n, automation, customer support
