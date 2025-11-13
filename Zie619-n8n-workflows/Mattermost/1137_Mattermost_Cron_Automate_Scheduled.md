# Workflow Analysis for Coffee Bot (Mattermost)

## Description
This workflow automates the process of organizing virtual coffee catch-ups for team members using Mattermost and Google Calendar.

## Input Details
The workflow is triggered automatically every Monday at 10 AM by a scheduled cron job.

## Process Summary
First, a greeting message is posted in a specified Mattermost channel. Then, it retrieves a list of all employees participating in the coffee chat channel. These employees are then randomly divided into groups, ideally of three people, ensuring no group has only one member. Finally, the workflow announces these newly formed groups in the Mattermost channel and simultaneously sends out Google Calendar invitations to all group members for a virtual coffee meeting.

## Output Details
The workflow posts group announcements in a Mattermost channel and creates Google Calendar events with meeting links for each group.

## Tags
automation, n8n, production-ready, excellent, optimized
