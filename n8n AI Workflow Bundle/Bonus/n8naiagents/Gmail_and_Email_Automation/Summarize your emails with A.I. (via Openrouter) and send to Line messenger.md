# Workflow Analysis for AI Email Summarizer and Messenger Notifier

## Description
This workflow automatically reads emails, uses an AI model to summarize them, and then sends the summarized content to a Line Messenger chat.

## Input Details
The workflow is triggered by reading emails from a configured IMAP email account.

## Process Summary
First, the workflow connects to an IMAP server and reads incoming emails. Next, it sends the email sender, subject, and HTML content to an AI model hosted on Openrouter.ai for summarization. The AI is instructed to highlight important information, action items, deadlines (in bold), and provide concise summaries for less important emails. Finally, the AI-generated summary is sent as a text message to a specific recipient on Line Messenger.

## Output Details
The workflow outputs summarized email content as text messages to a Line Messenger chat.
