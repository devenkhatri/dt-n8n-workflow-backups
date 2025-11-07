# Workflow Analysis for AI-Powered Outlook Email Categorization and Archiving

## Description
This workflow automatically categorizes incoming Outlook emails using AI and then organizes them into specific folders, applying appropriate categories within Outlook. It focuses on unflagged and uncategorized emails, streamlining email management for users.

## Input Details
The workflow is manually triggered and fetches unflagged and uncategorized emails from a specified Microsoft Outlook inbox.

## Process Summary
The workflow retrieves emails, then converts their HTML body to a clean, readable format suitable for AI processing. An AI agent (Ollama Chat Model) analyzes each email and assigns a primary category (e.g., "junk", "receipt", "SaaS", "community", "action", "business", or "other") and an optional subcategory. Based on the AI-assigned category, the workflow updates the email's categories in Outlook and moves it to a corresponding dedicated Outlook folder. Additionally, emails categorized as "action" or "business" that have been read are moved to an "Actioned" folder. Error handling is included to manage issues during AI output processing.

## Output Details
The workflow updates the categories of emails in Microsoft Outlook and moves them to specific Outlook folders (e.g., Junk Email, Receipt, SaaS, Community, Actioned) based on the AI-driven categorization.
