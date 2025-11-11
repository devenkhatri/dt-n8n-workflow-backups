# Workflow Analysis for The Recap AI - Gmail Agent

## Description
This workflow has two main functions: (1) It builds a structured knowledge base from a lawn care company's website by scraping all pages and using AI to organize the content into a standardized format, then saves it as a Google Doc; and (2) It automatically monitors incoming Gmail messages, analyzes them using the knowledge base, and sends intelligent replies when appropriate, while logging all activity to Google Sheets.

## Input Details
The workflow is triggered either by a web form submission containing a website URL and Google Drive folder ID, or by the receipt of a new email in a Gmail inbox.

## Process Summary
When triggered by the form, the workflow scrapes all URLs from the provided website using Firecrawl, initiates a batch scrape of those pages, and polls until completion. It then uses a powerful AI model to synthesize the scraped content into a structured lawn care business knowledge base in Markdown format. This knowledge base is converted to HTML, styled, and uploaded as a Google Doc to the specified Drive folder. Separately, when a new email arrives, the Gmail agent analyzes it, consults the knowledge base, decides whether to respond, sends an appropriate reply if needed, and logs the decision and action to Google Sheets.

## Output Details
The workflow produces a formatted Google Doc containing the synthesized knowledge base stored in a specified Google Drive folder, and optionally sends automated email replies while logging all email handling decisions and actions to a Google Sheet.

## Tags
AI Agent, Web Scraping, Knowledge Base, Gmail Automation, Google Drive, Google Sheets, Firecrawl, Content Synthesis, Email Auto-Reply, Lawn Care
