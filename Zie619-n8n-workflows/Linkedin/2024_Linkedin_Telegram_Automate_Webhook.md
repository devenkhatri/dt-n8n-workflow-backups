# Workflow Analysis for Linkedin Automation

## Description
This n8n workflow automates your LinkedIn posting by fetching articles from Medium.com twice a day, ensuring consistent content sharing without manual effort. To prevent duplicates, it stores posted article IDs in Airtable and sends a Telegram message after every successful post.

## Input Details
This workflow is triggered by a schedule, running daily at 9:00 AM and 7:00 PM UTC.

## Process Summary
The workflow begins by fetching a list of already posted article IDs from Airtable. It then randomly selects a tag and retrieves new article IDs from Medium.com based on this tag, filtering out any articles that have already been posted. For each new article, it fetches the full content and an image. If an image is available, it then publishes the article with its image to LinkedIn. Finally, it records the newly posted article's ID in Airtable and sends a success notification via Telegram.

## Output Details
The workflow publishes articles to LinkedIn, updates an Airtable database with the IDs of posted articles, and sends a Telegram notification to confirm successful posts.

## Tags
Automation, LinkedIn, Medium, Airtable, Telegram, Scheduled, Content Publishing, Social Media, Productivity
