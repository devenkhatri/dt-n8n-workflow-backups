# Workflow Analysis for Production Workflow

## Description
This workflow automatically checks a website daily at 1 PM UTC for trending 'Show HN' posts, extracts relevant details like title, URL, and ranking, and emails a formatted list of these posts if any are found.

## Input Details
The workflow is triggered daily at 1 PM UTC by a cron scheduler and fetches data from a web page specified by the BASE_URL environment variable.

## Process Summary
The workflow starts with a scheduled trigger at 1 PM UTC, then makes an HTTP request to a configured URL. It extracts HTML elements representing news items, parses each item to get the title, URL, and rank, and filters only those items whose title contains 'Show HN:'. If matching items are found, it formats them into an email body and sends the email.

## Output Details
The workflow sends an email with a list of currently trending 'Show HN' posts, including their rank, title, and URL, to a predefined recipient.

## Tags
automation, email notification, web scraping, scheduled workflow, Show HN, n8n, production-ready
