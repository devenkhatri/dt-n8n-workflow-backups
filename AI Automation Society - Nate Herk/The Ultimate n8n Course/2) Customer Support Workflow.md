# Workflow Analysis for Customer Inquiry Triage and Notification System

## Description
This workflow automatically processes incoming customer support inquiries, identifies if the customer is known or a VIP using an Airtable lookup, and then routes the corresponding high- or low-priority notifications to the appropriate internal Slack channels for immediate support team action.

## Input Details
The workflow is triggered by an incoming HTTP request via a Webhook, receiving data containing customer inquiry details such as name, email, subject, and message body.

## Process Summary
The workflow starts by receiving a customer support request via a Webhook, which is then parsed to extract key information. It then queries an Airtable base using the customer's email to determine if they are a known user. A conditional check routes the flow: if the customer is known, it checks for a 'VIP' tag and sends a high-priority notification to a specific Slack channel. If the customer is known but not a VIP, or if they are a completely new customer, a standard notification is sent to a general support channel. Finally, a confirmation email is sent back to the customer acknowledging receipt of their request.

## Output Details
The workflow produces internal notifications routed to different Slack channels based on customer status (VIP, known, or new), and it sends an automated acknowledgment email back to the customer.
