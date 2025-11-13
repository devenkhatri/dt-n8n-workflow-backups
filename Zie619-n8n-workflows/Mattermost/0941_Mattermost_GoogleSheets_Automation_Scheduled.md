# Workflow Analysis for StatsInstagram

## Description
This workflow automatically retrieves and reports Instagram statistics.

## Input Details
This workflow is triggered daily at 8 AM by a Cron schedule.

## Process Summary
First, the workflow is triggered by a daily schedule. It then gets the current date and formats it. Next, it reads Instagram statistics like account name, followers, and posts from a Google Sheet. Finally, it composes a message with these statistics and sends it to a specified Mattermost channel.

## Output Details
The workflow sends an informative message with Instagram statistics to a Mattermost channel.

## Tags
automation, n8n, production-ready, excellent, optimized
