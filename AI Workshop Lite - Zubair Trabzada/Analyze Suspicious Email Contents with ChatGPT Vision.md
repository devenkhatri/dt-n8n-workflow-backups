# Workflow Analysis for Phishing Email Detection and Jira Ticket Creation

## Description
This workflow automatically detects incoming emails from Gmail or Outlook, analyzes them for potential phishing attempts using AI, and creates a detailed Jira ticket with the email content, headers, and a screenshot for security review.

## Input Details
The workflow is triggered by new emails arriving in a Gmail inbox (checked every minute); Outlook email trigger is configured but currently disabled.

## Process Summary
When a new Gmail email arrives, key details like subject, recipient, HTML body, and headers are extracted and standardized. The HTML body is sent to hcti.io to generate a screenshot of the email. The screenshot and email headers are then analyzed by ChatGPT-4 to assess phishing risk. A Jira ticket is created with the email details and AI analysis, and the screenshot is attached to the ticket for visual reference.

## Output Details
The workflow creates a Jira ticket in the 'Support' project with a summary, detailed description including AI analysis, and attaches a screenshot of the suspicious email.

## Tags
phishing detection, email security, Gmail, Outlook, Jira integration, AI analysis, ChatGPT, email screenshot, security automation, threat response
