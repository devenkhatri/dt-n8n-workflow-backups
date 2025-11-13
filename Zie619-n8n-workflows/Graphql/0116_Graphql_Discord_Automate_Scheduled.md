# Workflow Analysis for Cron Workflow

## Description
This workflow automatically fetches the top 5 ranked Product Hunt projects from the last 24 hours and posts their details to a Discord channel every hour.

## Input Details
The workflow is triggered automatically every hour by a cron scheduler and does not require external input data.

## Process Summary
The workflow starts with a cron trigger that runs hourly. It then queries a GraphQL API to fetch the top 5 Product Hunt posts from the last 24 hours based on ranking. The response is transformed into a list of individual posts using an item list node. A Set node extracts key fields (Name, Description, Votes) from each post. Finally, the extracted data is sent to a Discord channel via a webhook.

## Output Details
The workflow sends a formatted message containing the name, description, and vote count of each top Product Hunt project to a configured Discord webhook.

## Tags
automation, cron, graphql, discord, product hunt, scheduled workflow, n8n
