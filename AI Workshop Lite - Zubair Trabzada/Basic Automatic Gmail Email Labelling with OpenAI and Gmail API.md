# Workflow Analysis for Gmail Email Auto-Labeling with AI

## Description
This workflow automatically categorizes incoming Gmail emails by analyzing their content and assigning them to existing labels or creating new, appropriately structured labels when needed.

## Input Details
The workflow is triggered by new emails arriving in a Gmail inbox, polling every 5 minutes via the Gmail API.

## Process Summary
The workflow first detects a new email using a Gmail trigger. It then passes the email to an AI agent that reads the message content and fetches all existing Gmail labels. The AI analyzes the email's subject, sender, and body to determine the best matching label. If no suitable label exists, it creates a new one following the existing naming conventions and label hierarchy. Finally, it assigns the appropriate label(s) to the email and removes the inbox label for less important messages like promotions.

## Output Details
The workflow labels the Gmail message with either an existing or newly created label, organizing the inbox automatically.

## Tags
gmail, email automation, AI labeling, OpenAI, inbox management, email categorization
