# Workflow Analysis for Effortless AI-Powered Email Management

## Description
This workflow automates the handling of incoming emails, summarizes their content, generates appropriate responses using a retrieval-augmented generation (RAG) approach, and obtains human approval or suggestions before sending replies.

## Input Details
The workflow is primarily triggered by new emails received via an IMAP account. It also has a manual trigger for setting up and refreshing the knowledge base.

## Process Summary
The workflow starts by reading an incoming email via IMAP and converting its content to Markdown. An AI model then summarizes this email, and a separate AI agent drafts a professional reply, utilizing a Qdrant vector store as a company knowledge base. This draft is sent to a designated Gmail address for human review and approval. Based on the human's feedback, a text classifier determines if the email is approved or declined. If declined, an AI email reviewer revises the draft using the feedback, and it's re-sent for review; if approved, the final email is sent to the original sender. A separate initialization path handles creating and populating the Qdrant knowledge base from Google Drive documents.

## Output Details
The workflow produces a drafted email for human review and, upon approval, sends the final AI-generated reply to the original sender.
