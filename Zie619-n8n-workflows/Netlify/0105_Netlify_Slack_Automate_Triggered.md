# Workflow Analysis for Netlify Deploy Failure Notification

## Description
This workflow automatically notifies relevant stakeholders when a Netlify site deployment fails, providing essential details about the failure.

## Input Details
The workflow is triggered by a Netlify webhook when a deployment fails for a configured site, receiving information about the failed deploy.

## Process Summary
1. The workflow starts when Netlify reports a deployment failure for a specific site.
2. It then extracts details about the failed deployment, including the site name and error message.
3. Finally, it constructs a message containing these details.
4. This message is then sent to a designated Slack channel.

## Output Details
The workflow sends a detailed notification about the failed Netlify deployment to a specified Slack channel.

## Tags
automation, n8n, production-ready, excellent, optimized
