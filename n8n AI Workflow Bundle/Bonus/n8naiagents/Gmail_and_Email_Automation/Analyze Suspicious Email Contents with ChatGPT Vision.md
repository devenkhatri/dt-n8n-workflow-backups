# Workflow Analysis for Email Phishing Report Automation with AI Analysis and Jira Integration

## Description
This workflow automatically processes incoming emails (currently from Gmail) to detect potential phishing attempts. It generates a visual screenshot of the email, uses AI to analyze its content and headers for phishing indicators, and then creates a detailed Jira ticket with the analysis and screenshot attached for further investigation.

## Input Details
The workflow is triggered every minute by new emails received in a connected Gmail account; a Microsoft Outlook trigger is also configured but currently disabled.

## Process Summary
The workflow listens for new incoming emails from Gmail (or optionally Outlook). It extracts key email details such as HTML body, text body, subject, recipient, and headers. The HTML content of the email is then sent to an external service to generate a screenshot, which is subsequently retrieved. An AI model (ChatGPT) analyzes both the email's screenshot and its headers to identify potential phishing characteristics and generate an assessment. Finally, a new Jira ticket is created, summarizing the reported phishing email, including the recipient, subject, email body, and the AI's detailed analysis, with the email screenshot attached.

## Output Details
The workflow creates a new Jira ticket containing details of the suspicious email, an AI-generated phishing analysis, and an attached screenshot of the email.
