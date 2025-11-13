# Workflow Analysis for AccountCraft WhatsApp Automation - Infridet

## Description
This workflow automatically captures new leads and engages them through email and WhatsApp, while also logging their information in Google Sheets and updating their status in a CRM system.

## Input Details
The workflow is triggered by a webhook that receives lead data (name, email, and phone number) from a form or external source.

## Process Summary
When a new lead is submitted via the webhook, the workflow first logs the lead details into a Google Sheet for backup. It then adds the lead as a contact in FluentCRM with a 'New Lead' tag. Next, it sends a warm welcome email and a personalized WhatsApp message to the lead. Finally, it updates the lead's tag in the CRM to 'Customer' to reflect their status after initial contact.

## Output Details
The workflow logs leads in Google Sheets, adds and updates contacts in FluentCRM, sends a welcome email, and delivers a WhatsApp message to the lead.

## Tags
lead capture, CRM integration, WhatsApp automation, email automation, Google Sheets logging, marketing automation, n8n workflow
