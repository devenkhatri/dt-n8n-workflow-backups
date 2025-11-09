# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) It creates a structured knowledge base from a lawn care company's website by scraping all pages and organizing the content into a comprehensive document stored in Google Drive, and (2) It monitors a Gmail inbox to automatically respond to customer inquiries about services, pricing, and policies using the knowledge base, while logging all email interactions to Google Sheets.

## Input Details
The workflow is triggered either by a form submission containing a website URL and Google Drive folder ID (for knowledge base creation) or by receiving a new email in a Gmail account (for the email agent functionality).

## Process Summary
For knowledge base creation: The workflow scrapes all URLs from the submitted website using Firecrawl, performs a batch scrape of the content, waits for completion, then uses an LLM to synthesize the scraped content into a structured knowledge base following strict formatting guidelines. The resulting document is converted to HTML and uploaded to Google Drive. For email handling: The workflow monitors incoming Gmail messages, analyzes each email using an AI agent that consults the knowledge base, decides whether to respond based on content relevance, sends automated replies when appropriate, and logs all decisions and actions to Google Sheets.

## Output Details
The workflow produces a structured knowledge base document in Google Drive and optionally sends automated email replies to customers while logging all email processing activities to Google Sheets.

## Tags
knowledge base, web scraping, Gmail automation, AI agent, Google Drive, Google Sheets, lawn care, customer support, LLM, document generation
