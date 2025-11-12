# Workflow Analysis for Email AI Auto-responder. Summerize and send email

## Description
This workflow automatically responds to incoming emails by summarizing their content, classifying them as company information requests, and generating a professional, context-aware reply using AI. It leverages a knowledge base stored in a vector database to ensure accurate and relevant responses.

## Input Details
The workflow is triggered by incoming emails received via IMAP to a monitored inbox (e.g., info@n3witalia.com).

## Process Summary
The workflow first converts the HTML email body into Markdown for better LLM processing. It then uses DeepSeek R1 to summarize the email content in under 100 words. The summary is classified to ensure it is a 'Company info request'—only such emails proceed further. The system retrieves relevant information from a Qdrant vector store (populated from Google Drive documents) to inform the response. Finally, a draft reply is generated, reviewed and formatted in HTML by a separate AI model, and sent back to the original sender.

## Output Details
The workflow sends an automated, AI-generated, HTML-formatted reply email to the original sender, using the monitored inbox's SMTP credentials.

## Tags
email automation, AI assistant, email summarization, auto-responder, vector database, Qdrant, company knowledge base, n8n, production-ready
