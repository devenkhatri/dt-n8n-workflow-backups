# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically monitors incoming emails from Gmail (and optionally Outlook), analyzes them using AI to detect potential phishing threats, and creates detailed Jira tickets with email content and screenshots for security review.

## Input Details
The workflow is triggered by new emails arriving in a Gmail inbox, polled every minute; it receives full email data including subject, body (HTML and plain text), headers, and recipient information.

## Process Summary
The workflow starts by capturing new Gmail messages and extracting key email fields into structured variables. It converts the email body to a text file and generates a visual screenshot of the HTML content using an external API. The email content and headers are then sent to ChatGPT for AI-powered phishing analysis, which returns a structured verdict (malicious or benign) with a detailed explanation. Based on this verdict, the workflow creates an appropriate Jira ticket in the Support project and attaches both the email screenshot and text body for further investigation.

## Output Details
The workflow outputs a Jira ticket (either 'Potentially Malicious' or 'Potentially Benign') with a detailed AI-generated analysis, along with attached screenshot and text file of the email, enabling security teams to review and act on reported emails.

## Tags
email security, phishing detection, Gmail automation, AI analysis, Jira integration, n8n workflow, automated ticketing, email monitoring
