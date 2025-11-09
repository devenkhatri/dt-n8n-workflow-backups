# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) it builds a structured knowledge base from a lawn care company's website by scraping all pages and using AI to organize the content into a comprehensive document saved to Google Drive, and (2) it automatically monitors incoming Gmail messages, analyzes them against the knowledge base, and sends helpful replies when appropriate while logging all activity to Google Sheets.

## Input Details
The workflow is triggered either by a form submission containing a website URL and Google Drive folder ID to build a knowledge base, or by a received Gmail message to potentially generate an automated response.

## Process Summary
When building a knowledge base, the workflow maps all URLs from the provided website, scrapes them in batch, waits for completion, then uses an AI model to synthesize the content into a structured markdown document following strict formatting rules for lawn care businesses. This knowledge base is converted to HTML and saved as a Google Doc in the specified folder. Separately, when an email is received, a Gmail agent analyzes it using AI, checks against the knowledge base, decides whether to respond, sends a helpful reply if appropriate, and logs all actions to Google Sheets.

## Output Details
The workflow produces a comprehensive knowledge base document stored in Google Drive when building from a website, and for email processing, it either sends automated Gmail replies or logs decisions to a Google Sheet.

## Tags
knowledge base, web scraping, AI, Gmail automation, Google Drive, Google Sheets, lawn care, document generation, email response, LLM
