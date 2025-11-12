# Workflow Analysis for Slack Workflow

## Description
This workflow demonstrates multiple automation examples including sending Slack messages, categorizing emails with AI, building a RAG system with PDFs and Pinecone, and an AI appointment booking assistant that interacts with a calendar.

## Input Details
The workflow is triggered by multiple inputs: a webhook (for Slack/email processing), incoming Gmail messages (disabled), and chat messages via a public chat interface for appointment booking.

## Process Summary
The workflow begins by receiving data through a webhook and checks if the email contains '@n8n'. If so, it sends a message to a Slack channel. Separately, it includes an email categorization flow using AI to label Gmail messages as 'automation' or 'music'. Another section downloads a PDF (e.g., Bitcoin whitepaper), splits its text, generates embeddings using OpenAI, and stores them in Pinecone. A chat interface allows users to ask questions about the PDF using a retrieval-augmented generation (RAG) pipeline. Finally, an AI agent powered by Anthropic helps users book 30-minute appointments by checking calendar availability and creating events via API calls.

## Output Details
The workflow outputs include Slack messages, Gmail labels, data stored in Pinecone, chat responses from AI, and calendar appointments booked via API.

## Tags
Slack, AI, RAG, PDF, Pinecone, Chatbot, Email Automation, Calendar Booking, n8n, Webhook
