# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically monitors incoming Gmail (and optionally Microsoft Outlook) emails, analyzes them using AI to detect potential phishing threats, and creates detailed Jira tickets with email screenshots and body attachments for security review.

## Input Details
The workflow is triggered by new incoming emails in a Gmail account (checked every minute); optionally, it can also be triggered by Microsoft Outlook emails (currently disabled).

## Process Summary
The workflow starts by capturing new emails via the Gmail Trigger node and extracts key details like subject, recipient, HTML body, and headers using the Set Gmail Variables node. It then converts the email body into a text file and generates a visual screenshot of the HTML email using an external API. The email content and headers are sent to ChatGPT for AI-powered phishing analysis, which returns a structured verdict on whether the email is malicious. Based on this verdict, the workflow creates either a 'Potentially Malicious' or 'Potentially Benign' ticket in Jira, attaching both the email screenshot and the raw email body as files for further investigation.

## Output Details
The workflow creates a Jira ticket (either malicious or benign) with a detailed AI-generated analysis, and attaches both a screenshot of the email and its raw text body for security team review.

## Tags
email security, phishing detection, Gmail automation, AI analysis, Jira integration, email monitoring, n8n workflow, security automation
