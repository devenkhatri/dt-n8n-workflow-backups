# Workflow Analysis for Slack Workflow

## Description
This workflow demonstrates multiple automation examples including sending Slack messages, categorizing emails with AI, building a RAG system with PDFs and Pinecone vector storage, and creating an AI appointment booking assistant that interacts with a calendar API.

## Input Details
The workflow is triggered by multiple sources: a webhook that receives email query data, a Gmail trigger for new emails (currently disabled), a chat message webhook for appointment booking, and predefined PDF metadata for the RAG example.

## Process Summary
The workflow starts by processing incoming webhook data to check if an email contains '@n8n' and sends a message to Slack if true. In another branch, it categorizes incoming emails using AI and labels them in Gmail accordingly. A third branch downloads a PDF (like the BTC whitepaper), splits its text, creates embeddings with OpenAI, and stores them in Pinecone. Finally, a chat interface allows users to ask questions about the PDF or book appointments with an AI assistant that checks calendar availability and schedules meetings via API calls.

## Output Details
The workflow sends messages to Slack, adds labels to Gmail messages, stores document embeddings in Pinecone vector database, and enables an AI chat interface that can answer questions about stored documents or book calendar appointments via API responses.

## Tags
Slack, AI, RAG, Pinecone, PDF processing, email classification, calendar booking, webhook, OpenAI, Anthropic, vector database, automation, n8n
