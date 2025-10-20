# Workflow Analysis for Daily Time Report Generation and Distribution

## Description
This workflow generates a daily report of work items by employees, calculates their billed and unbilled time, and then sends individual reports to each employee via email and a compiled report to a designated team channel in Microsoft Teams.

## Input Details
The workflow is triggered daily at 8:00 AM by a Cron node, indicating a scheduled report generation.

## Process Summary
The workflow starts by fetching all "Work Items" from ClickUp. It then filters these work items to include only those updated today. Next, it aggregates and formats the data to calculate billed and unbilled time per employee. After that, it generates individual markdown reports for each employee and a consolidated markdown report for the team. Finally, it sends these individual reports via Outlook email and the consolidated report to a Microsoft Teams channel.

## Output Details
The workflow sends personalized daily work item reports to employees via Outlook email and a comprehensive team report to a Microsoft Teams channel.
