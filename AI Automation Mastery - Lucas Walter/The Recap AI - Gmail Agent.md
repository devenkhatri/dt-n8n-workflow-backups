# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow builds a structured knowledge base from a lawn care company's website and uses it to automatically respond to customer emails with accurate, up-to-date information about services, pricing, and policies.

## Input Details
The workflow is triggered either by a manual form submission containing a website URL and Google Drive folder ID, or by a new email arriving in a monitored Gmail inbox.

## Process Summary
When triggered by a form, the workflow scrapes the entire website using Firecrawl, processes the content with an AI model to generate a structured knowledge base based on specific guidelines, converts it to HTML, and saves it as a Google Doc in the designated Drive folder. When triggered by an email, it analyzes the message to determine if it's a service-related inquiry, checks whether the knowledge base contains sufficient information to provide an accurate response, sends a professional email reply if appropriate, and logs all decisions and actions to a Google Sheet for tracking and auditing purposes.

## Output Details
The workflow produces a Google Doc containing a structured knowledge base saved in a specified Google Drive folder and may send automated email responses to customers, while all email processing decisions are logged to a Google Sheet.

## Tags
knowledge base, web scraping, AI, Gmail automation, Google Drive, Google Sheets, customer support, lawn care, email auto-reply, Firecrawl
