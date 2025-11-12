# Workflow Analysis for Auto Categorise Outlook Emails with AI

## Description
This workflow automatically categorizes unread, unflagged Outlook emails that don’t already have categories using an AI model. It sanitizes email content, sends it to an AI agent for analysis, and then updates the email with appropriate categories and moves it to a matching folder (e.g., Junk, Receipt, SaaS, Community, Actioned, or Business).

## Input Details
The workflow is triggered manually and processes emails from a specified Outlook inbox folder, filtering for emails that are unflagged and have no existing categories.

## Process Summary
The workflow fetches unprocessed Outlook emails, converts their HTML body to clean text, and prepares key fields like subject and sender. It then sends this sanitized data to an AI model (Ollama) with strict instructions to categorize the email into one of predefined categories. The AI’s JSON response is parsed, validated, and used to update the email’s categories in Outlook. Based on the category, the email is moved to a corresponding folder (e.g., 'Junk Email', 'Receipt', 'SaaS'). If the email is already read, it’s moved to an 'Actioned' folder.

## Output Details
The workflow updates each email with AI-determined categories and moves it to a designated Outlook folder based on its category.

## Tags
Outlook automation, AI email categorization, Ollama, email management, n8n workflow, no-code automation, Microsoft Outlook integration, AI agent, email filtering, productivity automation
