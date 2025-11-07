# Workflow Analysis for Financial News Recap Workflow

## Description
This workflow automates the daily delivery of curated financial news via email to a designated recipient. It fetches financial news articles from a website, extracts specific content, summarizes it using an AI model, and then sends the summary in an HTML-formatted email via Microsoft Outlook.

## Input Details
This workflow is triggered daily at 7:00 AM by a scheduled trigger.

## Process Summary
First, the workflow fetches the HTML content from ft.com. Then, it extracts specific news headlines and sections using CSS selectors. The extracted news content is then gathered into a single text. An AI agent, powered by the Google Gemini Chat Model, summarizes this collected financial news into a structured HTML format, designed to provide investors with a clear market overview. Finally, the HTML-formatted summary is sent as an email via Microsoft Outlook.

## Output Details
The workflow produces a summarized HTML-formatted financial news report which is sent as an email via Microsoft Outlook.
