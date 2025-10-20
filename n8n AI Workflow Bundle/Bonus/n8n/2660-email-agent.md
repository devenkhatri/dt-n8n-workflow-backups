# Workflow Analysis for AI Email Agent with n8n & Google Gemini

## Description
This workflow automates email processing using AI. It fetches emails from Gmail, summarizes them using Google Gemini, categorizes them, extracts action items, drafts replies, and sends them, improving efficiency and response times for customer support and sales.

## Input Details
The workflow is triggered manually and processes emails from a specified Gmail inbox.

## Process Summary
The workflow first fetches unread emails from a Gmail inbox. Next, it processes each email by using Google Gemini to summarize the email content, categorize the email as support, sales, or other, and extract any action items. Subsequently, it drafts a reply using Gemini based on the email content and categorization. Finally, it sends the drafted reply via Gmail, marking the original email as read.

## Output Details
The workflow sends AI-generated email replies via Gmail and marks the processed emails as read in the Gmail inbox.
