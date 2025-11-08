# Workflow Analysis for Auto Categorise Outlook Emails with AI

## Description
This workflow automatically fetches unflagged and uncategorized emails from Microsoft Outlook, uses an AI model to categorize them based on their content, and then updates the email's category in Outlook and moves it to a designated folder according to the AI's classification.

## Input Details
The workflow is manually triggered and fetches unflagged and uncategorized emails from a specified Microsoft Outlook folder.

## Process Summary
The workflow starts by fetching one unflagged and uncategorized email at a time from a specific Outlook folder. For each email, it first sanitizes the email body by converting HTML to markdown and removing unnecessary characters, then extracts key fields like subject, sender, and importance. An AI agent (Ollama Chat Model) analyzes the sanitized email content, subject, and sender, classifying it into one of several predefined categories such as "action", "junk", "receipt", "SaaS", "community", "business", or "other". The AI's categorized output is then parsed, and based on the assigned category, the workflow updates the email's category in Outlook. Finally, the email is moved to a corresponding Outlook folder (e.g., Junk Email, Receipt, SaaS, Community, Actioned) or a general folder if it requires action and is already read.

## Output Details
The workflow updates the categories of Outlook emails and moves them to specific Outlook folders based on the AI-driven categorization.
