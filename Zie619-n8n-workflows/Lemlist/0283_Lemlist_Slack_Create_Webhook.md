# Workflow Analysis for Lemlist Workflow

## Description
This workflow automates lead management based on email replies received via Lemlist, categorizing responses and triggering appropriate actions in CRM and communication tools.

## Input Details
This workflow is triggered by new email replies from leads within Lemlist campaigns.

## Process Summary
The workflow begins by categorizing the content of a lead's email reply using OpenAI, classifying it as "Unsubscribe," "Interested," "Out of Office," or "Other." Based on this categorization, the workflow takes different paths: for "Unsubscribe" replies, it unsubscribes the lead in Lemlist; for "Interested" replies, it marks the lead as interested in Lemlist, creates a new deal and retrieves contact information in HubSpot, then sends a notification to Slack; for "Out of Office" replies, it retrieves contact information and creates a follow-up task in HubSpot. Additionally, a general Slack notification is sent for every lead reply, regardless of its category.

## Output Details
The workflow unsubscribes leads in Lemlist, marks leads as interested, creates deals and follow-up tasks in HubSpot, and sends notifications to Slack channels.

## Tags
automation, n8n, lemlist, hubspot, openai, slack, lead management, email automation, production-ready
