# Workflow Analysis for Auto Categorise Outlook Emails with AI

## Description
This workflow automatically categorizes new Outlook emails using a local AI model (Ollama) and organizes them into predefined folders like 'Actioned', 'Junk', 'Receipt', 'SaaS', 'Community', or 'Business' based on their content.

## Input Details
The workflow is triggered manually or automatically and fetches unread, unflagged, and uncategorized emails from a specified Outlook folder using a filter query.

## Process Summary
The workflow retrieves eligible Outlook emails, sanitizes their content by removing HTML and markdown, and passes the cleaned text to an AI agent powered by Ollama. The AI categorizes each email into one of six predefined categories and optionally a subcategory. Based on the AI's output, the workflow updates the email's category tags and moves it to the appropriate Outlook folder. If the email is already marked as read, it gets moved to the 'Actioned' folder.

## Output Details
The workflow updates each email with appropriate category tags and moves it to a designated Outlook folder (e.g., Junk, Receipt, SaaS, Community, Business, or Actioned) based on the AI's classification.

## Tags
Outlook, AI, Email Automation, Categorization, Ollama, n8n, Workflow Automation
