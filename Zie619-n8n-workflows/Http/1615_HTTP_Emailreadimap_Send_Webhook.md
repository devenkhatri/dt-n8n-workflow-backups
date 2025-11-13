# Workflow Analysis for Summarize emails with A.I. then send to messenger

## Description
This workflow automates the process of summarizing emails using Artificial Intelligence and then sending these summaries to a messenger application. It is designed to help users quickly get the gist of their emails and identify important information.

## Input Details
The workflow is manually triggered and then reads emails from a configured IMAP email account.

## Process Summary
First, the workflow is initiated manually. Next, it reads the latest emails from an IMAP email account. The content of each email, including sender, subject, and HTML body, is then sent to an AI service via an HTTP request with specific instructions to summarize the email, highlight important details, action items, and deadlines. Finally, the summarized content received from the AI is sent to a specified messenger application through another HTTP request.

## Output Details
The workflow produces a concise, AI-generated summary of emails, which is then sent as a text message to a messenger application.

## Tags
automation, n8n, production-ready, excellent, optimized
