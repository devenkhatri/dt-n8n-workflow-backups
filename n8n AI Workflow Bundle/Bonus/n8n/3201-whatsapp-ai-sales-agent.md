# Workflow Analysis for WhatsApp AI Sales Agent

## Description
This workflow automates customer interactions on WhatsApp using AI to answer queries and qualify leads, then notifies a sales team for follow-up.

## Input Details
The workflow is triggered by an incoming WhatsApp message received via a webhook.

## Process Summary
First, the workflow extracts the sender's phone number and the message content. It then fetches contact details from HubSpot and prior conversation history. An AI model processes the current message, contact data, and history to generate a response, classify intent, and determine if the lead is qualified. If the lead is qualified, the workflow updates HubSpot and sends an internal notification to the sales team. Finally, an AI-generated response is sent back to the customer via WhatsApp.

## Output Details
The workflow sends AI-generated responses back to the WhatsApp sender, updates contact information in HubSpot, and sends internal notifications to a sales team regarding qualified leads.
