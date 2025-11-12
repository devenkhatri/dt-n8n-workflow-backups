# Workflow Analysis for Pipedrive Workflow

## Description
This workflow automatically qualifies leads who reply to cold email campaigns by analyzing their responses with AI. If a lead shows interest in a meeting, the workflow creates a new deal in Pipedrive CRM.

## Input Details
The workflow is triggered by incoming emails from one or more Gmail inboxes, specifically replies to cold outreach emails.

## Process Summary
The workflow starts by monitoring Gmail inboxes for new emails. It captures the email content and searches for the sender in Pipedrive CRM using their email address. It checks if the contact is part of a campaign and, if so, sends the email reply to OpenAI’s GPT-4 to assess interest in a meeting. The AI response is parsed to extract a yes/no interest flag and reason. If the lead is interested, a new deal is created in Pipedrive linked to that person.

## Output Details
If a lead is deemed interested, a new deal is created in Pipedrive CRM; otherwise, no action is taken.

## Tags
CRM, lead qualification, email automation, AI analysis, Pipedrive, Gmail, OpenAI, sales automation
