# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow creates a structured knowledge base from a lawn care company's website and uses it to automatically respond to customer emails with accurate information about services, pricing, and policies.

## Input Details
The workflow is triggered either by a manual form submission with a website URL and Google Drive folder ID, or by a new email arriving in a monitored Gmail inbox.

## Process Summary
When triggered by a form, it scrapes the entire website using Firecrawl, processes the content with an AI model to create a structured knowledge base following specific guidelines, converts it to HTML, and saves it as a Google Doc in the specified Drive folder. When triggered by an email, it analyzes the message to determine if it's a service-related inquiry, checks if the knowledge base contains sufficient information to answer it accurately, sends a professional reply if appropriate, and logs all decisions and actions to Google Sheets for tracking.

## Output Details
The workflow generates a Google Doc containing a structured knowledge base in a specified Drive folder and optionally sends automated email responses to customers while logging all email processing decisions to a Google Sheet.

## Tags
knowledge base, web scraping, AI, Gmail automation, Google Drive, Google Sheets, customer support, lawn care, email auto-reply, Firecrawl
