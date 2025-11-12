# Workflow Analysis for Monitor Competitor Pricing

## Description
This workflow automatically tracks competitor pricing by fetching pricing page URLs from a Google Sheet, analyzing each page for plan details and price changes, updating the sheet with the latest pricing information, and sending a Slack alert whenever significant pricing changes are detected.

## Input Details
The workflow is triggered manually and receives competitor pricing URLs and previous pricing data from a Google Sheet.

## Process Summary
The workflow starts by fetching competitor pricing URLs and existing pricing data from a Google Sheet. It then uses an AI-powered extraction tool (Airtop) to analyze each pricing page, summarizing plan details and comparing them to previously recorded pricing. The AI response is parsed to extract structured fields like pricing summary, differences, and change status. Entries marked as 'SIMILAR' are filtered out, while 'DIFF' or 'NEW' entries update the Google Sheet with fresh pricing data and trigger a Slack notification to a designated channel.

## Output Details
The workflow updates the Google Sheet with the latest pricing summaries and timestamps, and sends Slack alerts for significant pricing changes to the 'pricing-changes' channel.

## Tags
automation, competitor monitoring, pricing analysis, Google Sheets, Slack notifications, AI extraction, production-ready
