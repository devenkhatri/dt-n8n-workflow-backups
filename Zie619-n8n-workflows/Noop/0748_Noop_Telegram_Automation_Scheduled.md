# Workflow Analysis for RSS to Telegram

## Description
This workflow automatically monitors a specified RSS feed for new entries and publishes them to a Telegram channel. It prevents duplicate posts by tracking the last successfully processed item.

## Input Details
The workflow is triggered by a scheduled cron job and reads data from a specified RSS feed URL.

## Process Summary
The workflow starts on a predefined schedule. It then fetches the latest items from the configured RSS feed. A function node retrieves the timestamp of the last processed RSS item from the workflow's static data. An If node compares the publication date of each RSS item with this timestamp, processing only newer items. Another function node updates the last read timestamp with the date of the newest processed item. Finally, a Telegram node sends a formatted message with the title and link of the new RSS item to a Telegram chat.

## Output Details
The workflow sends messages containing the title and link of new RSS feed items to a configured Telegram chat.

## Tags
automation, n8n, production-ready, excellent, optimized, RSS, Telegram, feed, news, notifications
