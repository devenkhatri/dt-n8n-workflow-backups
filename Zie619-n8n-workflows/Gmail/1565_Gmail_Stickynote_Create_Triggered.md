# Workflow Analysis for Save New Sales Opportunities

## Description
This workflow automatically captures sales-related emails labeled in Gmail, summarizes their content using AI, and creates a new sales opportunity in Odoo with the email details and summary.

## Input Details
The workflow is triggered by new emails in Gmail that have a specific sales-related label.

## Process Summary
The workflow starts by monitoring Gmail for emails with a designated sales label. When such an email arrives, it extracts the subject and sender's email address. It then uses an AI model (OpenAI) to generate a concise summary of the email content, highlighting key details like budget, timeline, and industry. Finally, it creates a new sales opportunity in Odoo using the email subject as the opportunity name, the sender's email as the contact, and the AI-generated summary as the description.

## Output Details
The workflow creates a new sales opportunity record in Odoo containing the email subject, sender's email, and an AI-generated summary of the inquiry.

## Tags
sales automation, email processing, Odoo integration, AI summarization, Gmail trigger, CRM, lead capture
