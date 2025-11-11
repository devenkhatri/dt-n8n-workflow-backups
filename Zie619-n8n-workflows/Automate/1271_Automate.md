# Workflow Analysis for Lead Processing and Notification Workflow

## Description
This workflow automatically processes new leads from a system like ERPNext, determines if they are relevant to the company's products or services, identifies the appropriate internal contact(s), and sends a formatted notification email summarizing the lead details. Invalid leads (e.g., job inquiries) are filtered out.

## Input Details
The workflow is triggered by a POST webhook containing new lead data from ERPNext, including lead name, company, source, notes, city, country, and mobile number.

## Process Summary
First, the workflow receives lead data via a webhook. It uses an AI model to analyze the lead notes and determine if the inquiry is valid (related to products, services, or solutions). If valid, it queries a Google Sheet (acting as a contact database) to find the appropriate internal contact(s) responsible for that area. It then generates a professional email notification summarizing the lead details using a predefined template. Finally, it formats the email body as HTML and sends the email via Microsoft Outlook.

## Output Details
The workflow sends a formatted HTML email notification to the relevant internal team member(s) via Microsoft Outlook, or discards the lead if it is deemed invalid.

## Tags
lead processing, AI analysis, email notification, CRM integration, Google Sheets, Microsoft Outlook, webhook automation, ERPNext
