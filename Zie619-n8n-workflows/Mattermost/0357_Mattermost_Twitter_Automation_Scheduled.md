# Workflow Analysis for Twitter notifications

## Description
Automated workflow: Twitter notifications. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered every minute by a scheduled cron job to search for tweets.

## Process Summary
The workflow initiates a search on Twitter for recent tweets containing "n8n_io". It then extracts specific tweet information such as ID, URL, tweet content, username, profile picture, name, and profile link color. A function node filters these tweets to identify and process only new, previously unsent tweets. Finally, it sends these new tweet details as a formatted message to a designated Mattermost channel.

## Output Details
The workflow sends new tweet notifications, including links and content, to a specified Mattermost channel.

## Tags
automation, n8n, production-ready, excellent, optimized
