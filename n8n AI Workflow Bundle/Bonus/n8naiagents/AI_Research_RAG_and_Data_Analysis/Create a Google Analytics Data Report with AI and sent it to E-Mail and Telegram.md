# Workflow Analysis for Weekly Google Analytics Comparison Report

## Description
Every week the workflow pulls Google Analytics metrics for the last 7 days and the same 7‑day period from the previous year, summarizes the numbers, lets an AI generate a formatted HTML report with a short analysis, then emails the report and also sends a plain‑text version via Telegram.

## Input Details
A weekly schedule trigger (every Monday at 07:00) starts the workflow automatically.

## Process Summary
1) The trigger fetches current‑week GA4 metrics and maps them to readable fields; 2) the data is aggregated (sums and averages). 3) A code node calculates the matching dates from the previous year, pulls the same GA metrics for that period, maps and aggregates them. 4) An OpenAI model creates an HTML report comparing both periods with a brief summary. 5) The HTML is emailed and also converted to plain text by another AI model for a Telegram message.

## Output Details
The workflow sends a formatted HTML email report to a specified address and a plain‑text Telegram message to a chat.
