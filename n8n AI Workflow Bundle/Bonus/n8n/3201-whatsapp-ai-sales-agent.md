# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI to answer questions, record customer details, and notify sales teams for complex queries, enhancing customer service and lead management.

## Input Details
This workflow is triggered by an incoming message to a WhatsApp business account, specifically messages that are not status updates.

## Process Summary
The workflow begins by checking if the incoming WhatsApp message is a status update; if not, it proceeds. The AI then processes the message to answer the query, extracts entities like customer name and email, and stores them. If the AI cannot answer the question, it escalates the query by notifying the sales team via Slack and providing all available customer information. Finally, it sends the AI-generated response or an escalation message back to the customer on WhatsApp.

## Output Details
The workflow either sends an AI-generated answer directly to the WhatsApp user or sends a notification to the sales team via Slack for escalation.
