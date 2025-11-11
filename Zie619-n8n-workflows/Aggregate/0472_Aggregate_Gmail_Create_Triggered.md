# Workflow Analysis for Add AI labels to Gmail messages

## Description
This workflow automatically assigns custom labels to incoming Gmail messages based on their content using AI. It analyzes the email body with an OpenAI model, determines the appropriate label(s) (e.g., 'Partnership', 'Inquiry', or 'Notification'), and applies them directly in Gmail.

## Input Details
The workflow is triggered by new incoming Gmail messages via a Gmail polling trigger.

## Process Summary
The workflow starts by detecting a new Gmail message. It then retrieves the full message content using the message ID. This content is sent to an OpenAI model (gpt-4o-mini) with a system prompt instructing it to classify the message into predefined labels. The AI's JSON response is parsed to extract the label names. The workflow then fetches all existing Gmail labels, matches the AI-assigned label names to their corresponding Gmail label IDs, aggregates those IDs, and finally applies them to the original email message.

## Output Details
The workflow adds the appropriate Gmail label(s) to the incoming email message based on AI-generated classification.

## Tags
Gmail, AI labeling, OpenAI, email automation, n8n, workflow automation, message classification
