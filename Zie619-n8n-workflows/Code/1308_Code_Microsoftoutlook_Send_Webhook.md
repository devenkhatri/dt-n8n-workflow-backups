# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically detects incoming emails from Gmail (and optionally Microsoft Outlook), captures their content and headers, generates a screenshot of the email, analyzes it using AI for phishing indicators, and creates a detailed Jira ticket with the analysis and screenshot attached for security review.

## Input Details
The workflow is triggered by new incoming emails in a Gmail account (checked every minute); an Outlook email trigger is configured but currently disabled.

## Process Summary
When a new Gmail message arrives, the workflow extracts its HTML body, text body, subject, recipient, and headers. It then sends the HTML body to an external service (hcti.io) to generate a screenshot of the email. The generated image is retrieved and renamed. The email data, including headers and screenshot, is sent to ChatGPT for AI-powered phishing analysis. Finally, a Jira ticket is created with all relevant email details, the AI analysis, and the screenshot attached for security team review.

## Output Details
The workflow creates a Jira ticket in the 'Support' project with a summary, detailed description including email content and AI analysis, and attaches a screenshot of the email.

## Tags
email automation, phishing detection, Gmail integration, Jira integration, AI analysis, security workflow, n8n
