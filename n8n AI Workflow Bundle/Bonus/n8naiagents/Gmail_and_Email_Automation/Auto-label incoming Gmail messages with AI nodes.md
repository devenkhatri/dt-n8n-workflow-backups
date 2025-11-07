# Workflow Analysis for AI-Powered Gmail Message Labeling

## Description
This workflow automates the categorization of incoming Gmail messages by using Artificial Intelligence. It analyzes the content of new emails and assigns predefined labels like "Partnership", "Inquiry", or "Notification", helping users to automatically organize their inbox based on email content.

## Input Details
The workflow is triggered by new incoming messages in Gmail, polling every minute for new emails and receiving their IDs and basic information.

## Process Summary
The workflow starts by detecting new messages in Gmail and fetching their content. An AI model then analyzes the email content to assign relevant labels such as "Partnership", "Inquiry", or "Notification". Next, it retrieves all existing Gmail labels, merges them with the AI-assigned labels, and extracts their IDs. Finally, the workflow adds the determined labels to the original Gmail message.

## Output Details
The workflow updates the original Gmail message by adding AI-determined labels to it.
