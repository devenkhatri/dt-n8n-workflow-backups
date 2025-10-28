# Workflow Analysis for Daily AI Grants Discovery & Email Newsletter

## Description
This workflow automatically searches Grants.gov for new AI‑focused grant opportunities each morning, uses OpenAI to summarize their content and evaluate eligibility for your company, stores the results in Airtable, and then sends a concise HTML newsletter to your subscribed team members.

## Input Details
Triggered twice a day by scheduled timers—one at 8:30 AM for pulling new grants, another at 9:00 AM for compiling and sending the daily email. Input data comes from Grants.gov API responses and the Airtable tracker.

## Process Summary
1. At 8:30 AM a scheduled trigger requests the most recent AI grants from Grants.gov.
2. Grants are split into individual items and duplicate grant IDs are filtered out using the Remove Duplicates node.
3. For each new grant, a detailed payload is fetched, then OpenAI models generate a simplified synopsis and an eligibility assessment.
4. The combined information is merged and written as a new row in the Airtable tracker.
5. At 9:00 AM another scheduled trigger pulls grants marked "New" and "Eligible" from Airtable, builds an HTML email listing them, retrieves the active subscriber list, and emails each subscriber the newsletter.

## Output Details
Stores processed grant rows in Airtable and dispatches a daily HTML email newsletter via Gmail to active subscribers.
