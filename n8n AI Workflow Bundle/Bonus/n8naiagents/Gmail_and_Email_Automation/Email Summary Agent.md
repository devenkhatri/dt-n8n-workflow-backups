# Workflow Analysis for Email Summary Agent

## Description
This workflow automates the process of summarizing daily emails. It fetches all emails received in the last 24 hours from a specified email address, uses AI to create a summary with key details and action items, and then sends this organized summary in an HTML email to a designated team.

## Input Details
The workflow is triggered daily at 7 AM and receives email data from a specified Gmail account, specifically emails received in the past 24 hours.

## Process Summary
The workflow is initiated every day at 7 AM by a schedule trigger. It then fetches all emails received in the last 24 hours from a connected Gmail account. Next, it organizes the fetched email data, extracting specific fields such as the email ID, sender, recipient, CC list, and a snippet of the email content. After organizing, the workflow sends this aggregated email data to OpenAI (using the 'gpt-4o-mini' model) to generate a structured summary, identifying key details, issues, and action items. Finally, it constructs an HTML email containing the AI-generated summary and action items.

## Output Details
The workflow sends an HTML email containing the summarized emails and extracted action items to a specified team email address (e.g., team-email@example.com) and a CC list.
