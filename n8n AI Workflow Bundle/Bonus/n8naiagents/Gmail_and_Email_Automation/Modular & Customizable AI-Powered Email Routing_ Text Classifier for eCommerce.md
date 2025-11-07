# Workflow Analysis for Contact Form Text Classifier for eCommerce

## Description
This workflow automates the classification of contact form submissions and routes them to the appropriate department via email, while also logging the details in a Google Sheet. It is ideal for eCommerce businesses or customer support teams looking to streamline their contact form handling.

## Input Details
The workflow is triggered by a form submission, receiving the customer's Name, Email, and Message.

## Process Summary
First, the workflow receives a contact form submission containing the sender's name, email, and message. Next, an AI-powered text classifier analyzes the message and categorizes it into "Request Quote", "Product info", "General problem", "Order", or "other". Based on the classification, the workflow sends an email to the relevant internal department (e.g., Quote Department for quote requests, Product Department for product inquiries). Concurrently, the original contact form data, along with the assigned category, is recorded in a Google Sheet for logging and tracking purposes.

## Output Details
The workflow sends a categorized email to the relevant department and appends the contact form submission data to a Google Sheet.
