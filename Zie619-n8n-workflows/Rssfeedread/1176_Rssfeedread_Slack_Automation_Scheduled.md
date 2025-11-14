# Workflow Analysis for Post RSS feed items from yesterday to Slack

## Description
This workflow automatically fetches RSS feed items published yesterday and posts them to a designated Slack channel.

## Input Details
The workflow is triggered automatically every morning at 8 AM by a scheduled cron job.

## Process Summary
First, the workflow determines yesterday's date. Then, it retrieves items from a specified RSS feed. It filters these items to include only those published after yesterday. Finally, it formats the selected RSS items into a concise message.

## Output Details
The workflow sends the formatted message containing yesterday's RSS feed items to the '#news' channel in Slack.

## Tags
automation, n8n, production-ready, excellent, optimized, RSS, Slack, daily report
