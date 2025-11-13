# Workflow Analysis for Production Workflow

## Description
This workflow checks for new GitHub notifications every minute and sends a summary to a Discord channel if any are found.

## Input Details
The workflow is triggered every minute by a cron job and dynamically calculates the time range for checking new GitHub notifications.

## Process Summary
The workflow starts by calculating the timestamp for one minute ago. It then makes an authenticated HTTP request to a GitHub API endpoint to fetch notifications since that time. The response is processed to format each notification with its reason, title, and URL. If any notifications are found, a message is constructed; otherwise, nothing is sent. Finally, if there are notifications, the workflow sends a formatted message to a Discord channel mentioning a specific user.

## Output Details
When new GitHub notifications are detected, the workflow sends a formatted message to a Discord channel with links and details of each notification.

## Tags
GitHub, Discord, notifications, cron, automation, production
