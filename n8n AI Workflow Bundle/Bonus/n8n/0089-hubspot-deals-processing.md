# Workflow Analysis for HubSpot Deal Processing and Notification

## Description
This workflow processes new or updated deals in HubSpot, checks a custom property, and sends a Slack notification if the deal meets specific criteria.

## Input Details
The workflow is triggered by an HTTP webhook that receives deal data from HubSpot.

## Process Summary
The workflow starts by receiving deal data from HubSpot via a webhook. It then extracts the custom property "to_be_processed" from the deal. Following this, the workflow checks if the "to_be_processed" property is set to "true". If it is "true", a Slack message is sent to a specified channel, notifying about the deal. If it's "false", the workflow concludes without sending a Slack message.

## Output Details
The workflow sends a Slack notification to a specified channel if a HubSpot deal meets certain criteria.
