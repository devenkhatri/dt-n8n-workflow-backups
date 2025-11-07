# Workflow Analysis for AI-Powered Phishing Email Analysis and Jira Ticketing

## Description
This workflow automatically analyzes incoming emails for potential phishing threats using AI and creates corresponding support tickets in Jira, attaching email details and a visual screenshot for review.

## Input Details
The workflow is triggered every minute by new emails received in a connected Gmail account, receiving the email's full content including HTML body, text body, subject, recipient, and headers.

## Process Summary
First, the workflow extracts detailed information from the incoming email and consolidates it. Next, it converts the email's text body into a file and generates a visual screenshot of its HTML content using an external API. The email's HTML body and headers are then sent to ChatGPT for an AI-powered analysis to determine if it is a phishing attempt, providing a summary of its findings. Based on the AI's assessment, the workflow conditionally creates either a "Potentially Malicious" or "Potentially Benign" task in Jira. Finally, it attaches both the email screenshot and the raw text body of the email as files to the newly created Jira ticket for further investigation.

## Output Details
The workflow creates a Jira task, categorized as either "Potentially Malicious" or "Potentially Benign," containing the AI analysis summary, a screenshot of the email, and the raw text body of the email as attachments.
