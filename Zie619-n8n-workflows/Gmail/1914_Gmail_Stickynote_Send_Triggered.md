# Workflow Analysis for (G) - Email Classification

## Description
This workflow automatically classifies incoming Gmail messages into predefined categories such as High Priority, KS Work Related, Promotion, or Other using an AI-powered classification agent. Based on the classification, it labels the emails in Gmail accordingly to help prioritize and organize the inbox efficiently.

## Input Details
The workflow is triggered by new emails arriving in a Gmail inbox, polling every minute for unread messages.

## Process Summary
The workflow starts by polling Gmail for new emails. Each email's content is passed to a Classification Agent that uses a large language model (Google Gemini) to categorize the message into one of four predefined types. Depending on the assigned category, the workflow adds the corresponding Gmail label (e.g., 'High Priority', 'KS Work Related') to the email. Several sticky notes provide setup instructions for configuring labels, credentials, and classification rules. Error handling is included to manage execution failures.

## Output Details
The workflow adds appropriate Gmail labels to incoming emails based on their AI-determined classification, helping the user organize and prioritize their inbox.

## Tags
email automation, Gmail integration, AI classification, LLM, n8n, production-ready, workflow automation, email labeling
