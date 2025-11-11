# Workflow Analysis for Email Triage Agent (with Gmail)

## Description
This workflow automatically categorizes incoming unread Gmail messages by analyzing their content and applying relevant labels to keep the inbox organized.

## Input Details
The workflow is triggered by new unread emails in a Gmail inbox, polling every minute for unread messages.

## Process Summary
When a new unread email arrives, the workflow first retrieves all existing Gmail labels. It then uses an AI language model (GPT-4.1-mini) to analyze the email's sender, subject, and content. Based on this analysis, the AI selects 1–3 relevant labels and applies them to the email using Gmail’s labeling tool.

## Output Details
The workflow updates the original email in Gmail by attaching appropriate labels based on its content.

## Tags
gmail, email automation, AI classification, inbox organization, labeling
