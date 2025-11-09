# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow creates a structured knowledge base from a lawn care company's website and uses it to power an intelligent Gmail agent that automatically responds to customer inquiries when possible, while logging all interactions for tracking.

## Input Details
The workflow is triggered either by a form submission containing a website URL and Google Drive folder ID to build a knowledge base, or by a new incoming Gmail message that needs to be analyzed and potentially responded to.

## Process Summary
When building a knowledge base, the workflow scrapes all website pages using Firecrawl, extracts full content, and uses AI to synthesize it into a structured document with specific formatting. This document is converted to HTML and saved as a Google Doc in the specified Drive folder. When processing emails, the workflow analyzes incoming Gmail messages using an AI agent to determine if the query can be answered using the knowledge base. If appropriate, it retrieves the knowledge base, drafts a response, sends the email reply, and logs all actions and decisions to Google Sheets.

## Output Details
The workflow creates a structured knowledge base document in Google Drive, optionally sends automated email replies to customers, and logs all email processing decisions and actions to a Google Sheet.

## Tags
knowledge base, web scraping, AI agent, Gmail automation, Google Drive, Google Sheets, email response, lawn care, Firecrawl, Gemini AI
