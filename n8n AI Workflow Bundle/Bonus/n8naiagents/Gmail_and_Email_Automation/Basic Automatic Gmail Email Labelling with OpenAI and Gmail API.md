# Workflow Analysis for AI-Powered Gmail Email Categorization and Labeling

## Description
This workflow automatically categorizes incoming Gmail emails using artificial intelligence. It analyzes email content, sender, and subject to assign an appropriate existing label or create a new, structured sub-label if no suitable one is found, helping to organize your inbox efficiently.

## Input Details
The workflow is triggered every 5 minutes by new emails received in a specified Gmail account.

## Process Summary
The workflow is initiated when a new email arrives in Gmail. After a brief wait, an AI agent analyzes the email's details, including subject, sender, recipient, and content. The agent first reads all existing Gmail labels to find the most relevant match. If a suitable label is found, the agent assigns it to the email, potentially removing the inbox label for less important messages. If no appropriate label exists, the agent creates a new sub-label, often under an "AI" main label, and then assigns this new label to the email.

## Output Details
The workflow categorizes and labels Gmail messages by either assigning existing labels or creating and applying new, structured sub-labels.
