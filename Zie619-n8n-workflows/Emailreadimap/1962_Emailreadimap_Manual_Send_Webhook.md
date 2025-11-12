# Workflow Analysis for Email AI Auto-responder. Summerize and send email

## Description
This workflow automatically reads incoming emails, summarizes their content, classifies them as company information requests, retrieves relevant knowledge from a vector database, drafts a professional reply using AI, reviews the response for clarity and formatting, and sends the reply back to the sender—all without human intervention.

## Input Details
The workflow is triggered by incoming emails to info@n3witalia.com via IMAP.

## Process Summary
The workflow starts by reading an incoming email and converting its HTML body to plain text using a Markdown node. It then summarizes the email content using the DeepSeek R1 LLM. The summarized text is classified to ensure it’s a 'Company info request'; only matching emails proceed. The system queries a Qdrant vector store (using OpenAI embeddings) to retrieve relevant company knowledge. An AI agent drafts a concise, professional reply, which is then reviewed and formatted in HTML by another LLM. Finally, the formatted response is sent as an email reply to the original sender.

## Output Details
The workflow sends an automated, AI-generated, HTML-formatted reply email to the original sender, using the same email thread (with 'Re:' subject prefix).

## Tags
email automation, AI autoresponder, email summarization, LLM, vector database, Qdrant, OpenAI, DeepSeek, n8n, production-ready
