# Workflow Analysis for Add AI labels to Gmail messages

## Description
This workflow automatically categorizes incoming Gmail messages using AI and applies appropriate labels based on the email content. It uses OpenAI's GPT model to analyze the message and assign one or more predefined labels like 'Partnership', 'Inquiry', or 'Notification'.

## Input Details
The workflow is triggered by new incoming Gmail messages detected via polling.

## Process Summary
The workflow starts by detecting a new Gmail message and fetching its full content. The message body is then sent to an OpenAI language model with a prompt instructing it to categorize the email into predefined labels. The AI's JSON response is parsed to extract the assigned labels. The workflow then retrieves all existing Gmail labels, matches the AI-assigned label names to their corresponding Gmail label IDs, and finally adds those labels to the original email message.

## Output Details
The workflow adds the appropriate Gmail labels to the incoming email message based on AI-generated categorization.

## Tags
Gmail, AI, OpenAI, Email Automation, Labeling, Categorization, n8n
