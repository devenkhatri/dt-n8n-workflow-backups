# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) It creates a structured knowledge base from a lawn care company's website by scraping all pages and using AI to organize the information into a comprehensive document stored in Google Drive; and (2) It acts as an intelligent Gmail agent that automatically analyzes incoming emails, determines if they can be answered using the knowledge base, sends appropriate replies when possible, and logs all email interactions to Google Sheets.

## Input Details
The workflow is triggered either by a form submission containing a website URL and Google Drive folder ID to build a knowledge base, or by receiving a new Gmail message to analyze and potentially respond to.

## Process Summary
For knowledge base creation, the workflow scrapes all URLs from the provided website using Firecrawl, retrieves the full content of each page, and uses an AI model to synthesize the information into a structured knowledge base following strict formatting guidelines. This knowledge base is then converted to HTML and saved as a Google Doc in the specified Drive folder. For email handling, the workflow triggers when a new email arrives, uses an AI agent to analyze whether the email contains questions answerable from the knowledge base, retrieves the knowledge base if needed, decides whether to respond, sends a reply if appropriate, and logs all actions to Google Sheets.

## Output Details
The workflow produces a structured knowledge base document in Google Drive and optionally sends email replies to customers while logging all email processing decisions and actions to a Google Sheet.

## Tags
knowledge base, web scraping, AI agent, Gmail automation, Google Drive, Google Sheets, email response, lawn care, Firecrawl, Gemini AI
