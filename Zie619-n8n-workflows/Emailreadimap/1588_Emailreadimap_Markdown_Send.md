# Workflow Analysis for AI Email processing autoresponder with approval (Yes/No)

## Description
This workflow automatically reads incoming business emails, summarizes them, generates a professional AI-powered reply using company knowledge from a vector database, and sends the draft to a Gmail inbox for human approval before sending the final response.

## Input Details
The workflow is triggered by incoming emails via IMAP from a corporate email address.

## Process Summary
The workflow starts by reading incoming emails via IMAP. It converts the email body to Markdown for better LLM processing, then summarizes the content using a summarization chain. An AI agent retrieves relevant company information from a Qdrant vector database using embeddings and generates a concise, professional HTML-formatted reply. The draft reply is sent to a Gmail account with a 'Send and Wait for Response' action that presents Yes/No approval buttons. Only if approved ('Yes'), the final reply is sent back to the original sender.

## Output Details
The workflow either sends an approved AI-generated email reply to the original sender or takes no action if denied; the draft with approval buttons is delivered to a designated Gmail inbox.

## Tags
email automation, AI response, RAG, approval workflow, IMAP, Gmail, vector database, Qdrant, summarization, n8n
