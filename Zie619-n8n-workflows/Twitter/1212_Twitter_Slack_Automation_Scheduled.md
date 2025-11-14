# Workflow Analysis for Scrape Twitter for mentions of company

## Description
This workflow automatically monitors Twitter for mentions of a specific company or term and notifies a designated Slack channel when new mentions are found.

## Input Details
The workflow is triggered every 10 minutes by a scheduled cron job.

## Process Summary
The workflow begins by setting up the target Slack channel and the Twitter search term. It then calculates a timestamp for the last 10 minutes. Subsequently, it searches Twitter for the last 50 mentions of the configured term. Each mention is filtered to include only those created since the last run. Finally, it extracts the tweet text and its URL.

## Output Details
The workflow posts new company mentions, including the tweet text and URL, to a specified Slack channel.

## Tags
Twitter, Slack, Monitoring, Social Media, Automation, N8N, Production-Ready
