# Workflow Analysis for Extranet Releases

## Description
This workflow automatically notifies the team via Slack whenever a new release is published in a specific GitHub repository.

## Input Details
The workflow is triggered by a GitHub 'release' event webhook from the 'Mesdocteurs/mda-admin-partner-api' repository.

## Process Summary
The workflow starts when a new release is created in the specified GitHub repository. It captures the release details such as repository name, tag name, description, and URL. These details are then formatted into a message and sent to the 'extranet-md' Slack channel using a configured Slack bot. If any error occurs during execution, the workflow halts and reports the error.

## Output Details
The workflow posts a formatted Slack message to the 'extranet-md' channel with information about the new GitHub release.

## Tags
github, slack, release notification, automation, webhook, extranet
