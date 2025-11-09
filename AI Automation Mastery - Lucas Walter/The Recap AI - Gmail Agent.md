# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow builds a structured knowledge base from a lawn care company's website and uses it to automatically respond to customer inquiries received via Gmail, while logging all interactions.

## Input Details
The workflow is triggered either by a manual form submission with a website URL and Google Drive folder ID, or by a new email arriving in a monitored Gmail inbox.

## Process Summary
For knowledge base creation, it scrapes all pages from the provided website using Firecrawl, processes the content with an AI model to create a structured document following specific formatting rules, converts it to HTML, and uploads it as a Google Doc. For email handling, it analyzes incoming messages to detect service-related questions, consults the knowledge base to determine if a confident response can be generated, sends a professional reply when appropriate, and logs all decisions and actions to Google Sheets.

## Output Details
The workflow creates a structured knowledge base as a Google Doc in a specified Drive folder and optionally sends automated email replies to customers while recording all email processing decisions in a Google Sheet.

## Tags
knowledge base, web scraping, AI, Gmail automation, Google Drive, Google Sheets, customer support, lawn care, email auto-reply, Firecrawl
