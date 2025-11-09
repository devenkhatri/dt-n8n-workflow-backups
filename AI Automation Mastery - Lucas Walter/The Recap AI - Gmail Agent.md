# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) It builds a structured knowledge base from a lawn care company's website by scraping all pages and using AI to organize the content into a comprehensive document stored in Google Drive, and (2) It monitors a Gmail inbox to automatically analyze incoming emails and respond to customer inquiries using the knowledge base, while logging all actions to Google Sheets.

## Input Details
The workflow is triggered either by a form submission containing a website URL and Google Drive folder ID to build a knowledge base, or by receiving a new email in a Gmail inbox for automated customer support.

## Process Summary
For knowledge base creation, the workflow first scrapes all URLs from the submitted website using Firecrawl, then performs a batch scrape to extract content in markdown format. It polls until the scrape completes, then uses an AI model to synthesize the scraped content into a structured knowledge base document following strict formatting guidelines. The resulting markdown is converted to HTML and uploaded as a Google Doc to the specified Drive folder. For email handling, the workflow analyzes incoming emails using an AI agent that consults the knowledge base document to determine if it can provide a helpful response, then either sends a reply or takes no action, while logging all decisions to Google Sheets.

## Output Details
The workflow produces a structured knowledge base Google Doc stored in the specified Drive folder, and for email processing, it either sends automated replies to customers or logs non-responses, with all actions recorded in a Google Sheets log.

## Tags
knowledge base, web scraping, AI, Gmail automation, customer support, Google Drive, Google Sheets, Firecrawl, document generation, email bot
