# Workflow Analysis for Gmail Auto-Labeling and AI Analysis

## Description
This workflow automates the process of labeling new Gmail emails based on their content and then processes specific emails using an AI model for summarization or sentiment analysis, finally updating the Gmail thread with the AI-generated label and response.

## Input Details
This workflow is triggered when a new email is received in Gmail.

## Process Summary
The workflow starts by retrieving new emails from Gmail. It then filters these emails to exclude those with existing labels. Next, for each relevant email, it extracts the subject and body, and uses an AI model to determine a suitable label based on the content. Subsequently, it filters the emails again, specifically selecting ones with the "n8n AI" label, and for these, it performs an AI chat task, either summarizing or performing sentiment analysis on the email body. Finally, it updates the original Gmail threads with both the AI-determined label and the AI-generated response, if applicable.

## Output Details
The workflow updates the original Gmail threads by applying an AI-determined label and optionally adding an AI-generated response directly to the email.
