# Workflow Analysis for From Zero to Inbox Agent

## Description
An automated Gmail workflow that categorizes incoming emails into support, billing, high priority, or promotional types, then takes appropriate actions like replying with an AI assistant, forwarding to a team, creating drafts, or marking as read.

## Input Details
The workflow is triggered by new emails arriving in a Gmail inbox.

## Process Summary
The workflow starts by monitoring incoming Gmail messages. Each email is classified into one of four categories (Customer Support, Finance/Billing, High Priority, or Promotion) using an AI-powered text classifier. Based on the category, the email is labeled accordingly and a specific action is taken: customer support emails get an automated reply from a friendly AI assistant, billing emails are forwarded to a finance team, high-priority emails generate a draft reply from a sarcastic AI persona, and promotional emails are simply marked as read.

## Output Details
The workflow produces labeled emails, automated replies or drafts, forwarded messages to internal teams, and updates email read status based on the category.

## Tags
gmail, email automation, AI classification, customer support, billing, high priority, promotion, n8n, langchain, openrouter
