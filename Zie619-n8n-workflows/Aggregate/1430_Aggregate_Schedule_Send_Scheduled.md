# Workflow Analysis for Email Summary Agent

## Description
This workflow automatically fetches emails received in the past 24 hours, summarizes their key points and action items using AI, and sends a polished HTML report to a team email every morning at 7 AM.

## Input Details
The workflow is triggered daily at 7 AM and fetches emails from a specified Gmail inbox received since the previous day.

## Process Summary
The workflow starts with a daily 7 AM trigger. It then fetches all emails from the past 24 hours from a specific Gmail account. The relevant email fields (ID, From, To, CC, snippet) are extracted and organized. An OpenAI model (gpt-4o-mini) processes this data to generate a structured summary and list of action items in JSON format. Finally, the results are formatted into a styled HTML email and sent to designated recipients.

## Output Details
The workflow produces a daily HTML-formatted email summary with key points and action items, which is sent to a team email address and CC’d stakeholders.

## Tags
email automation, AI summary, daily report, Gmail integration, OpenAI, n8n workflow, production-ready
