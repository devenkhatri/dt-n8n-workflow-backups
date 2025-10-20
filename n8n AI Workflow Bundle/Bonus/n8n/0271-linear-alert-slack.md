# Workflow Analysis for Linear Alert to Slack

## Description
This workflow listens for new issues in Linear and sends a notification to a specified Slack channel.

## Input Details
The workflow is triggered by an HTTP webhook which receives data, likely from Linear, upon new issue creation.

## Process Summary
The workflow starts by receiving issue data via a webhook. It then extracts specific details like the issue ID, title, and URL. Next, it constructs a formatted message containing these issue details. Finally, it sends this message as a notification to a designated Slack channel.

## Output Details
The workflow sends a formatted message containing new Linear issue details to a Slack channel.
