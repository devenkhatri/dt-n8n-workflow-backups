# Workflow Analysis for Effortless Email Management with AI

## Description
This workflow automatically handles incoming business emails by summarizing them, generating AI-powered draft replies using company knowledge, and sending those drafts for human approval before final delivery.

## Input Details
The workflow is triggered by new incoming emails via IMAP from a specified email account.

## Process Summary
When an email arrives, it is converted to Markdown for better AI processing, then summarized. An AI agent uses a company knowledge base (stored in Qdrant) to draft a professional reply. This draft is sent via Gmail for human review and approval. A text classifier determines if the human feedback approves the email or requests changes. If approved, the email is sent; if declined, another AI agent revises the draft based on the feedback before sending.

## Output Details
The workflow either sends the final approved email reply to the original sender or updates the draft based on human feedback and resends it.

## Tags
email automation, AI reply, email summarization, human-in-the-loop, Qdrant, OpenAI, Gmail, IMAP, RAG, n8n
