# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically detects incoming emails from Gmail or Microsoft Outlook, captures their content and headers, generates a visual screenshot of the email, analyzes it using AI to detect potential phishing attempts, and creates a detailed Jira ticket with the analysis and screenshot attached for security review.

## Input Details
The workflow is triggered by new emails arriving in either a Gmail inbox (active) or a Microsoft Outlook inbox (currently disabled), polling for new messages every minute.

## Process Summary
When a new email arrives, the workflow extracts key details like subject, recipient, body (HTML and plain text), and headers. It then sends the HTML body to an external service (hcti.io) to generate a screenshot of the email. The workflow retrieves the screenshot and uses ChatGPT-4 to analyze the email content and headers for signs of phishing. Finally, it creates a Jira ticket with all relevant information, including the AI analysis and the email screenshot as an attachment.

## Output Details
The workflow creates a Jira ticket in the 'Support' project with a summary, detailed description including email content and AI analysis, and attaches a screenshot of the email for visual reference.

## Tags
email automation, phishing detection, Gmail integration, Outlook integration, AI analysis, Jira integration, security monitoring, email screenshot, workflow automation
