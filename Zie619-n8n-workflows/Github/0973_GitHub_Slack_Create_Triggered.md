# Workflow Analysis for Github Star Notification Workflow

## Description
This workflow monitors the n8n GitHub repository for star events and sends a real-time notification to a Slack channel whenever a user stars or unstars the repository.

## Input Details
The workflow is triggered by GitHub webhook events of type 'star' on the n8n-io/n8n repository, receiving event data including the action type, sender info, and current star count.

## Process Summary
The workflow starts when a GitHub 'star' event occurs. It checks whether the action is 'created' (star added) or something else (assumed to be star removed). If a star is added, it sends a green-colored message to Slack's #general channel with the stargazer's info and updated star count. If a star is removed, it sends a red-colored message with similar details. An error handler stops execution and logs an error if any step fails.

## Output Details
The workflow sends formatted messages to the Slack #general channel indicating whether a GitHub star was added or removed, including user details and repository star count.

## Tags
github, slack, star notification, automation, webhook, n8n
