# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) It creates a structured knowledge base from a lawn care company's website by scraping all pages and using AI to organize the content into a comprehensive document stored in Google Drive; and (2) It automatically monitors incoming Gmail messages, analyzes them against the knowledge base, and sends professional replies when appropriate while logging all activities to Google Sheets.

## Input Details
The workflow receives input through two separate triggers: a web form that accepts a website URL and Google Drive folder ID for knowledge base creation, and a Gmail trigger that activates when new emails are received.

## Process Summary
For knowledge base creation: the workflow scrapes all URLs from the provided website using Firecrawl API, performs a batch scrape of the content, polls until completion, then uses an LLM to synthesize the scraped content into a structured, deduplicated knowledge base document which is converted to HTML and uploaded to Google Drive. For email handling: when an email arrives, an AI agent analyzes whether it contains questions answerable from the knowledge base, retrieves the knowledge base from Google Docs, determines if a response is appropriate, sends a reply if needed, and logs all decisions and actions to Google Sheets.

## Output Details
The workflow produces a structured knowledge base document saved to a specified Google Drive folder and automatically sends email replies to appropriate customer inquiries while logging all email processing activities to a Google Sheets document.
