# Workflow Analysis for 🤖Customer Support Email Agent

## Description
This workflow automatically processes incoming Gmail messages to determine if they are customer support related. If they are, it uses AI to research company policies and draft a professional, empathetic reply. If not, it sends a notification that the email isn't support-related.

## Input Details
The workflow is triggered by new emails received in a Gmail inbox, polling every minute for new messages.

## Process Summary
The workflow starts by polling Gmail for new emails. It extracts the email body, sender, and thread ID. An AI model then evaluates whether the email is customer support related based on predefined topics. If it is, an AI agent uses a vector store (Pinecone) of support documents to research and draft a reply, which is saved as a Gmail draft. If it's not support-related, a notification is sent via Telegram. The AI-generated response summary is also sent to Telegram.

## Output Details
For customer support emails, a draft reply is created in Gmail and a summary is sent to Telegram; for non-support emails, a notification is sent to Telegram.

## Tags
gmail, ai, customer support, email automation, openai, pinecone, telegram, langchain
