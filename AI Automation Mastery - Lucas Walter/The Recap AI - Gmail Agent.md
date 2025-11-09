# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) It builds a structured knowledge base from a lawn care company's website by scraping all pages and using AI to organize the content into a comprehensive document stored in Google Drive, and (2) It monitors a Gmail inbox to automatically respond to customer inquiries about services, pricing, or policies using the knowledge base, while logging all email interactions to Google Sheets.

## Input Details
The workflow is triggered either by a manual form submission containing a website URL and Google Drive folder ID, or by receiving a new email in a monitored Gmail account.

## Process Summary
For knowledge base creation: The workflow scrapes all URLs from the provided website using Firecrawl, processes the scraped content with an AI model to synthesize a structured knowledge base following strict formatting guidelines, converts the result to HTML, and uploads it as a Google Doc to the specified Drive folder. For email handling: The workflow analyzes incoming emails to determine if they contain service-related questions, consults the knowledge base to assess if it can provide an accurate response, sends a professional reply when appropriate, and logs all decisions and actions to Google Sheets.

## Output Details
The workflow produces a Google Doc containing a structured knowledge base uploaded to a specified Drive folder, and optionally sends automated email replies to customers while logging all email processing decisions to a Google Sheet.

## Tags
knowledge base, web scraping, AI, Gmail automation, Google Drive, Google Sheets, customer support, lawn care, email auto-reply, Firecrawl
