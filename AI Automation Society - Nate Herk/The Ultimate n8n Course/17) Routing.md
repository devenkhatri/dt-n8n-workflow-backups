# Workflow Analysis for Routing

## Description
This workflow automatically categorizes incoming Gmail messages into predefined categories (High Priority, Customer Support, Promotions, or Finance/Billing) using AI, then routes each email to a specialized AI agent that either responds directly or escalates urgent issues to a human via Telegram.

## Input Details
The workflow is triggered by new emails in a Gmail inbox and receives the full email content including sender, subject, body, and thread ID.

## Process Summary
The workflow starts by monitoring a Gmail account for new emails. Each incoming email is passed to an AI-powered text classifier that categorizes it into one of four predefined categories based on its content. Depending on the classification, the email is labeled in Gmail and routed to a specialized AI agent (High Priority, Customer Support, Promotion, or Finance). High-priority emails are summarized and escalated to a human via Telegram, while other categories trigger AI-generated email replies using appropriate brand personas. All AI agents use the same OpenAI language model for consistency.

## Output Details
The workflow labels emails in Gmail, sends AI-generated email replies for non-urgent categories, and escalates high-priority emails to a human via Telegram message.

## Tags
email routing, AI classification, Gmail automation, customer support, Telegram escalation, OpenAI integration
