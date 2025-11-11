# Workflow Analysis for Email Summary Agent

## Description
This workflow automatically fetches emails received in the past 24 hours, summarizes their key points and action items using AI, and sends a formatted HTML email report to specified recipients every morning at 7 AM.

## Input Details
The workflow is triggered daily at 7 AM and fetches emails received in the last 24 hours from the Gmail account isb.quantana@quantana.in.

## Process Summary
The workflow starts with a daily 7 AM trigger. It then fetches all emails received in the past 24 hours from a specific Gmail address. The email data is organized to extract key fields like sender, recipient, CC, and snippet. This organized data is sent to OpenAI’s GPT-4o-mini model to generate a structured summary and list of action items. Finally, the summary is formatted into an HTML email and sent to designated team and CC recipients.

## Output Details
The workflow produces a styled HTML email containing a summary of recent emails and associated action items, which is sent to team-email@example.com and cc-list@example.com.

## Tags
Product, AI, Building blocks, Finance, IT Ops, OpenAI, Marketing, Support, HR, Project Management, DevOps
