# Workflow Analysis for Activity Encouragement

## Description
This workflow is designed to encourage physical activity by monitoring Strava data and notifying accountability partners if a user's activity level falls below a set threshold. It's an automated, production-ready workflow with robust error handling and security features.

## Input Details
The workflow is triggered daily at 11:00 AM by a scheduled cron job and retrieves the user's latest activity data from Strava.

## Process Summary
The workflow starts daily at 11 AM. It initializes settings such as a minimum activity duration and the email addresses of the user and their accountability partners. It retrieves all recent activity data from the user's Strava account. It then evaluates if the user's total moving time from Strava meets or exceeds the predefined minimum activity duration. If the activity is insufficient, an email is composed and sent to the designated accountability partners.

## Output Details
If the user's activity is below the set threshold, an email is sent to predefined accountability partners to encourage the user.

## Tags
Automation, n8n, Production-ready, Excellent, Optimized, Strava, Fitness, Accountability, Email, Scheduled
