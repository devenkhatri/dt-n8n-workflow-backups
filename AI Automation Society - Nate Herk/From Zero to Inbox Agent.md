# Workflow Analysis for From Zero to Inbox Agent

## Description
This workflow automates inbox management by categorizing incoming Gmail messages using AI and then performing specific actions based on the classification. It streamlines responses for customer support, forwards billing inquiries, prioritizes urgent messages, and processes promotional content efficiently.

## Input Details
This workflow is triggered every minute by new emails received in a connected Gmail account, receiving the email's subject, body, and other header information.

## Process Summary
The workflow constantly monitors a designated Gmail inbox for new emails. Upon receiving an email, its subject and body are processed by an AI-powered Text Classifier, which assigns one of four categories: Customer Support, Finance/Billing, High Priority, or Promotion. Depending on the classification, the workflow takes a specific path: Customer Support emails are labeled and replied to by an AI assistant; Finance/Billing emails are labeled and forwarded to a dedicated billing address; High Priority emails are labeled and an AI assistant creates a draft response; Promotional emails are labeled and marked as read.

## Output Details
The workflow manages emails by replying to specific inquiries, forwarding others, creating draft responses, or marking them as read, while consistently applying category-specific labels in Gmail.
