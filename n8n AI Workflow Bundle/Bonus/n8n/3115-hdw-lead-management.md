# Workflow Analysis for HDW Lead Management

## Description
This workflow automates the processing and management of leads by capturing data from a webhook, enriching it with company information, and then notifying relevant parties.

## Input Details
The workflow is triggered by an authenticated webhook which receives lead data.

## Process Summary
The workflow starts by receiving lead data via a webhook. It then extracts specific data fields like full name, email, and company and searches for the company in Clearbit to gather additional company information. Subsequently, it prepares a message summarizing the lead details and sends this message to a specified Discord channel as a notification.

## Output Details
The workflow sends a formatted notification message containing lead and company details to a Discord channel.
