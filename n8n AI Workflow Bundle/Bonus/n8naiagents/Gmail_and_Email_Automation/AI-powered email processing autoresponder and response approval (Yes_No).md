# Workflow Analysis for AI Email Autoresponder with Approval

## Description
This workflow automates the process of handling incoming emails, summarizing their content using AI, generating intelligent replies with the help of a company knowledge base, and then sending these replies after a manual approval step.

## Input Details
The workflow is triggered by new emails received in a configured IMAP inbox, providing the email's content, subject, sender, and recipient.

## Process Summary
Upon receiving an email via IMAP, the workflow converts its HTML content to Markdown. An AI model then generates a concise summary of the email. An AI agent drafts a professional reply, leveraging a Qdrant Vector Store as a company knowledge base to provide relevant information. The generated email draft is sent to a designated Gmail address for manual approval (Yes/No). If approved, the workflow proceeds to send the final email reply to the original sender.

## Output Details
The workflow sends an approved, AI-generated email reply to the original sender from the IMAP account that initially received the email.
