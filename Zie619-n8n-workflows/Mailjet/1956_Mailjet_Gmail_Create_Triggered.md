# Workflow Analysis for Forward Netflix emails to multiple email addresses with GMail and Mailjet

## Description
This workflow automates the forwarding of Netflix emails to a predefined list of recipients using Gmail as the trigger and Mailjet for sending the emails.

## Input Details
The workflow is triggered every minute by new emails received in a Gmail account, specifically filtering for emails originating from "netflix.com".

## Process Summary
First, the workflow checks for new Netflix emails in the configured Gmail account. Next, it defines a static list of email addresses that will receive the forwarded email. Then, it splits the workflow items so that each recipient email address is processed individually. Finally, for each recipient, the original Netflix email content (HTML, text, and subject) is sent via Mailjet.

## Output Details
The workflow sends the received Netflix email to multiple specified email addresses using the Mailjet email service.

## Tags
automation, n8n, production-ready, excellent, optimized
