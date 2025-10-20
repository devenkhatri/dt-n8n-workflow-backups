# Workflow Analysis for Support Sales Flow

## Description
This workflow automates the process of handling incoming support tickets, categorizing them, and escalating sales-related inquiries.

## Input Details
The workflow is triggered by incoming emails received through a Mailman Webhook.

## Process Summary
The workflow starts by receiving an email. It then uses OpenAI to classify the email content as either "Sales" or "Support". If the email is classified as "Sales", it creates a new lead in HubSpot. If it is classified as "Support", it creates a new ticket in HubSpot and also logs the ticket in Google Sheets. Finally, it sends a confirmation email to the sender.

## Output Details
The workflow creates leads or tickets in HubSpot, logs support tickets in Google Sheets, and sends confirmation emails.
