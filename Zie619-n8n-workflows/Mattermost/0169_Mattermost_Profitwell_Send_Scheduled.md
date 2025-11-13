# Workflow Analysis for Send financial metrics monthly to Mattermost

## Description
Automated workflow: This workflow processes data and performs automated tasks by sending financial metrics monthly to Mattermost.

## Input Details
The workflow is triggered monthly at 9 AM by a cron schedule.

## Process Summary
First, the workflow is triggered monthly at 9 AM. Then, it retrieves monthly financial metrics from ProfitWell. Next, it sends these financial metrics, including active customers, new customers, growth rate, and recurring revenue, to a specified Mattermost channel as a message. Lastly, it includes an error handler to catch and report any workflow execution errors.

## Output Details
The workflow sends a message containing key financial metrics to a Mattermost channel.

## Tags
automation,n8n,production-ready,excellent,optimized
