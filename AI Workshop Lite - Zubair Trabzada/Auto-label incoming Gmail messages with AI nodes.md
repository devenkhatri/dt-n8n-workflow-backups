# Workflow Analysis for Automated Gmail Labeling with AI

## Description
This workflow automatically categorizes incoming Gmail messages and assigns relevant labels using artificial intelligence. It identifies messages related to partnerships, inquiries, or notifications.

## Input Details
The workflow is triggered every minute by new incoming messages in Gmail, receiving the message ID and other basic email metadata.

## Process Summary
First, the workflow retrieves the full content of a new Gmail message. It then sends this content to an AI model which categorizes the email and assigns predefined labels (Partnership, Inquiry, Notification). Next, it retrieves all existing labels from Gmail and merges them with the AI-assigned labels. Finally, it aggregates the IDs of all applicable labels and applies them to the original Gmail message.

## Output Details
The workflow updates the original Gmail message by adding relevant AI-determined labels to it.
