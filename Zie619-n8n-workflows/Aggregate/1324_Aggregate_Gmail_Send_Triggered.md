# Workflow Analysis for Gmailtrigger Workflow

## Description
This workflow automatically categorizes incoming Gmail messages by assigning relevant labels such as 'Partnership', 'Inquiry', or 'Notification' using AI. It retrieves new emails, analyzes their content with OpenAI's language model, matches the AI-suggested labels with existing Gmail labels, and applies them to the email.

## Input Details
The workflow is triggered by new incoming Gmail messages detected via a polling-based Gmail trigger.

## Process Summary
The workflow starts by detecting new Gmail messages. It then fetches the full message content and sends it to OpenAI's GPT model with instructions to classify the email into predefined labels. The AI response is parsed to extract label names. Meanwhile, the workflow retrieves all existing Gmail labels. It merges the AI-assigned label names with the actual Gmail label definitions, aggregates their corresponding label IDs, and finally applies those labels to the original Gmail message.

## Output Details
The workflow adds appropriate Gmail labels to the incoming email message based on its content.

## Tags
Gmail, AI, email automation, labeling, OpenAI, n8n, workflow automation
