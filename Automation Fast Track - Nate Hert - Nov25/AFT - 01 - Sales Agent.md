# Workflow Analysis for AFT - 01 - Sales Agent

## Description
An automated sales workflow that manages lead onboarding, follow-up sequences, call scheduling via Calendly, and no-show recovery—all using Google Sheets as a CRM.

## Input Details
The workflow is triggered by scheduled intervals and Calendly booking events, and receives lead data from a Google Sheets 'Lead List'.

## Process Summary
First, new leads from a Google Sheet are transferred to a CRM sheet and assigned unique IDs. Separately, every two days, the system identifies CRM contacts who have started a follow-up sequence but haven't booked a call, and sends them up to three personalized AI-generated emails. When someone books a 30-minute meeting via Calendly, their CRM record is updated to reflect the scheduled call. Additionally, every 6 hours, the system checks for leads marked as 'No' in the 'Showed Call?' column and sends them a no-show follow-up email.

## Output Details
The workflow updates Google Sheets CRM records, sends personalized follow-up emails via Gmail, and logs interactions like call scheduling and no-shows.

## Tags
sales automation, CRM, Google Sheets, email follow-up, Calendly integration, AI email generation, lead management, no-show recovery
