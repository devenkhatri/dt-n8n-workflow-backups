# Workflow Analysis for Automate Figma Versioning and Jira Updates with n8n Webhook Integration

## Description
This workflow automatically captures Figma design version updates and posts them as comments on corresponding Jira issues, keeping design and development teams aligned.

## Input Details
The workflow is triggered by a Figma webhook that fires whenever a file version is updated, providing details like page name, version name, design link, and associated Jira issue key.

## Process Summary
The workflow starts when a new Figma file version is published, triggering the Figma node. It then retrieves the relevant Jira issue using the issue key from the payload. Finally, it adds a comment to that Jira issue containing the page name, version notes, design link, and timestamp. A sticky note provides setup instructions for the Figma Commit Plugin, and an error handler manages failures.

## Output Details
The workflow posts a formatted comment with Figma version details to a specified Jira issue, ensuring design updates are logged directly in the development tracking system.

## Tags
automation, n8n, Figma, Jira, design workflow, version tracking, webhook, production-ready
