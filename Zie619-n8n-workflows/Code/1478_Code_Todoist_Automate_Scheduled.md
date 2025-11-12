# Workflow Analysis for Daily Digest Email Workflow

## Description
This workflow automatically compiles a daily digest email that includes your top tasks from Todoist, latest news from an RSS feed (Times of India), and recent emails from Gmail, then sends it to your inbox in a clean, styled HTML format.

## Input Details
The workflow is triggered on a scheduled basis (e.g., daily) and pulls data from an RSS feed, Gmail emails, and Todoist tasks.

## Process Summary
The workflow starts with a schedule trigger, then fetches the latest items from three sources: an RSS feed (Times of India), Gmail emails, and Todoist tasks. It limits each source to the top 5 items. A code node merges and formats this data into a styled HTML email body with a subject line. Finally, the formatted digest is sent via Gmail to a specified email address.

## Output Details
The workflow sends a richly formatted daily digest email to the user's Gmail inbox containing summarized tasks, news, and recent email snippets.

## Tags
daily digest, email automation, rss feed, gmail, todoist, html email, scheduled workflow, productivity, n8n
