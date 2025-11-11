# Workflow Analysis for Ahrefs Keyword Research Workflow

## Description
This workflow automates keyword research by accepting a user-provided keyword, cleaning and validating it, fetching detailed keyword data from the Ahrefs API (including search volume, competition, and CPC metrics), and formatting a human-readable summary of the main keyword and its top 10 related keywords.

## Input Details
The workflow is triggered manually or via a chat message input that contains a keyword phrase.

## Process Summary
First, a keyword is extracted and cleaned from the user input using an AI agent. This refined keyword is then sent to the Ahrefs API via an HTTP request to retrieve comprehensive keyword metrics. A code node processes the raw API response to extract the main keyword data and up to 10 related keywords with key fields like monthly searches and competition. The data is aggregated into a single JSON structure and passed to a response formatter. Finally, a Google Gemini AI model formats the data into a clear, readable text summary based on a predefined system message.

## Output Details
The workflow produces a well-formatted text summary of keyword research data, which can be sent back to the user via chat, email, or another communication channel.

## Tags
keyword research, SEO, Ahrefs, AI, Google Gemini, n8n, automation, API integration, content strategy, marketing
