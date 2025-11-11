# Workflow Analysis for Email Summary Agent

## Description
This workflow automatically fetches emails received in the last 24 hours from a specified inbox, summarizes their key points and action items using AI, and emails a formatted HTML summary to a team every morning at 7 AM.

## Input Details
The workflow is triggered daily at 7 AM and fetches emails from the 'isb.quantana@quantana.in' Gmail inbox received in the past 24 hours.

## Process Summary
The workflow starts with a daily 7 AM trigger. It then fetches all emails from the specified Gmail address received in the last 24 hours. Relevant email fields like sender, recipient, CC, and snippet are extracted and organized. The organized email data is sent to OpenAI (GPT-4o-mini) to generate a structured summary and list of action items. Finally, the results are formatted into a styled HTML email and sent to designated recipients.

## Output Details
The workflow sends a daily HTML-formatted email summary with key points and action items to 'team-email@example.com' (and CCs 'cc-list@example.com').

## Tags
email automation, AI summary, daily digest, Gmail integration, OpenAI, n8n workflow, production-ready
