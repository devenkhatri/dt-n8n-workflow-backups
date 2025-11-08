# Workflow Analysis for Email Triage Agent (with Gmail)

## Description
This workflow automates email organization by using an AI agent to categorize incoming Gmail messages and apply appropriate labels.

## Input Details
The workflow is triggered periodically (every minute) by new unread emails from a connected Gmail account.

## Process Summary
First, the workflow is activated when new unread emails arrive in Gmail. Next, an AI-powered email classification agent analyzes the email's sender, subject, and content. The agent utilizes a "Get all Labels" tool to fetch available Gmail labels and a language model to determine the most relevant categories. Finally, the agent employs an "Add Label" tool to assign 1-3 appropriate labels to the analyzed email within Gmail.

## Output Details
The workflow labels the processed emails in Gmail according to the AI agent's classification.
