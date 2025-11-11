# Workflow Analysis for Weekly UX Ideas Summary Reporter

## Description
This workflow automatically counts how many new UX-related product ideas have been added to a Notion database in the past week and posts a summary message to a Slack channel.

## Input Details
The workflow is triggered on a weekly schedule and optionally pulls recent entries from a Notion database (currently mocked with sample data).

## Process Summary
The workflow starts with a weekly schedule trigger. Instead of using the disabled Notion node, it uses a Code node to inject mock product idea data. It then filters this data to include only items tagged with 'UX'. Next, it uses the Item Lists node to count the unique number of UX ideas. Finally, it sends a formatted summary message to a specified Slack channel.

## Output Details
The workflow posts a message to a Slack channel announcing the number of new UX ideas added in the last 7 days.

## Tags
automation, Notion, Slack, scheduled report, UX research, data summary, n8n
