# Workflow Analysis for Customer Lead AI Agent Workflow

## Description
This workflow automatically processes new customer leads from a website, validates if the inquiry is relevant to the company's products or services, identifies the right internal contact(s) to handle it, and sends a professionally formatted email notification with lead details. Invalid or unrelated inquiries are filtered out.

## Input Details
The workflow is triggered by a webhook that receives new lead data from ERPNext when a lead is created with 'Website' as the source and 'Open' status.

## Process Summary
The workflow first filters leads from the website with open status, then retrieves full lead details from ERPNext. It checks if the lead includes notes, then passes the lead information to an AI agent (simulated via system prompt) that analyzes the inquiry, identifies relevant internal contacts from a Google Sheet, and generates a formatted email body. If the inquiry is valid, the workflow extracts email fields, converts the message to HTML, and sends it via Microsoft Outlook. Invalid leads are dropped.

## Output Details
For valid leads, the workflow sends a professional HTML email via Microsoft Outlook to the appropriate internal team member(s) with lead details and a link to the lead in ERPNext.

## Tags
lead processing, AI agent, email automation, ERPNext integration, customer inquiry, workflow automation, Microsoft Outlook, Google Sheets, lead qualification
