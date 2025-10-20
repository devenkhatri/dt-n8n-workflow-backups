# Workflow Analysis for Mattermost Financial Metrics Cron

## Description
This workflow retrieves financial metrics from an internal API and posts them as a formatted message to a Mattermost channel on a scheduled basis.

## Input Details
This workflow is triggered every weekday at 9 AM by a Cron node.

## Process Summary
The workflow starts by fetching financial statistics from a specified internal API endpoint. It then formats the retrieved data into a user-friendly message using an Edit Fields node to modify the JSON structure and a Code node to construct a Markdown message. Finally, it sends this formatted message to a designated Mattermost channel.

## Output Details
The workflow posts a formatted message containing financial statistics to a Mattermost channel.
