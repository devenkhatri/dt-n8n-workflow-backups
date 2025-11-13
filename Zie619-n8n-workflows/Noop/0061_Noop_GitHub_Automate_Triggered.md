# Workflow Analysis for Telegramtrigger Workflow

## Description
This workflow processes data received from Telegram and automates tasks, specifically for deploying a new version of n8n.

## Input Details
This workflow is triggered by messages received from Telegram, expecting a message containing "/deploy" followed by a version number.

## Process Summary
First, the workflow is activated when a message is received in Telegram. It then checks if the message text contains the word "/deploy". If it does, the workflow extracts the version number from the message. Finally, it uses this version number to create a new release on GitHub for the "n8n" repository owned by "n8n-io".

## Output Details
The workflow creates a new release on GitHub, specifically for the n8n repository.

## Tags
automation, n8n, production-ready, excellent, optimized
