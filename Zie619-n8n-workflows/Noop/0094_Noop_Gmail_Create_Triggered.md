# Workflow Analysis for Hubspot Workflow

## Description
This automated workflow processes data received from Typeform and performs various tasks in Hubspot and Gmail.

## Input Details
This workflow is triggered by new submissions from a Typeform and receives form submission data.

## Process Summary
The workflow starts by extracting and setting specific values from the Typeform submission. It then creates a new contact in Hubspot using this information. An "If" condition checks if the lead is interested. If interested, the contact's lifecycle stage in Hubspot is updated to "opportunity", and a personalized email with scheduling and presentation links is sent via Gmail. If not interested, a NoOp node is executed, concluding the process.

## Output Details
The workflow either creates/updates a contact in Hubspot and sends an email via Gmail to interested leads, or simply creates a contact in Hubspot for non-interested leads.

## Tags
automation,n8n,production-ready,excellent,optimized,Typeform,Hubspot,Gmail,CRM,Lead Management,Email Automation
