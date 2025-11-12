# Workflow Analysis for Auto Categorise Outlook Emails with AI

## Description
This workflow automatically categorizes incoming Outlook emails using an AI model. It processes unread, unflagged, and uncategorized emails, cleans their content, sends them to an AI agent for classification, and then updates the email with appropriate categories and moves it to the correct folder (e.g., Junk, Receipt, SaaS, Community, Actioned, or Business).

## Input Details
The workflow is triggered manually and pulls emails from a specified Outlook inbox folder, filtered to include only unread, unflagged, and uncategorized messages.

## Process Summary
The workflow starts by fetching eligible Outlook emails based on specific filters. It then sanitizes each email’s body by stripping HTML and unnecessary formatting. The cleaned email data is passed to an AI agent (simulated via a prompt) that categorizes the email into predefined types like 'junk', 'receipt', 'SaaS', etc., optionally assigning a subcategory. The AI’s JSON-formatted response is parsed, and based on the category, the email is updated with tags and moved to a corresponding Outlook folder (e.g., 'Junk Email', 'Receipt', 'Actioned'). Error handling ensures failed AI parsing doesn’t stop the workflow.

## Output Details
The workflow updates each processed email in Outlook with AI-determined categories and moves it to a specific folder based on its classification.

## Tags
email automation, AI categorization, Outlook integration, n8n workflow, email management, no-code automation, AI agent, email filtering
