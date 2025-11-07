# Workflow Analysis for Summarize emails with A.I. then send to messenger

## Description
This workflow reads emails, uses an AI to summarize their content, and then sends these summaries to a messenger application, allowing users to quickly grasp important information without manually sifting through all emails.

## Input Details
The workflow is triggered by the "Read emails (IMAP)" node, which continuously checks and receives incoming emails from a configured IMAP account.

## Process Summary
First, the workflow reads emails from a specified IMAP account. Next, it sends the email details (sender, subject, and HTML content) to an AI model via Openrouter.ai for summarization. The AI is prompted to identify important emails, highlight urgent items with emojis, extract action items and deadlines in bold, and provide concise summaries. Finally, the AI-generated summarized content is sent as a text message to a designated user on the Line messenger platform.

## Output Details
The workflow produces AI-generated summaries of emails and sends them as text messages to a specific recipient on the Line messenger platform.
