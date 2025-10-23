# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using an AI sales agent. It uses a custom set of instructions and a knowledge base to answer customer questions and provide support, escalating to a human agent when necessary.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
The workflow starts by extracting the customer's message and contact information from the incoming WhatsApp message. It then uses a custom system prompt and the message history to interact with an AI sales agent, which determines the appropriate response or action. If the AI determines a human agent is needed, it notifies the sales team via Slack and creates a lead in Zoho CRM. Otherwise, the AI generates a response, potentially using a knowledge base for additional information, and sends it back to the customer via WhatsApp.

## Output Details
The workflow sends automated responses to customers on WhatsApp, notifies a sales team on Slack if human intervention is required, and creates leads in Zoho CRM for follow-up.
