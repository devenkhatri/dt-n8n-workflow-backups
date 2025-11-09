# Workflow Analysis for AFT - 01 - Sales Agent

## Description
An automated sales workflow that manages leads through multiple stages: importing new leads into a CRM, sending up to three AI-personalized follow-up emails at scheduled intervals, updating CRM status when prospects book calls via Calendly, and re-engaging no-shows with a follow-up email.

## Input Details
The workflow is triggered by scheduled intervals for lead processing and follow-ups, Calendly event bookings for call scheduling, and manual CRM updates for no-shows.

## Process Summary
First, new leads from a Google Sheet are transferred to a CRM sheet and assigned unique IDs. Concurrently, the system checks existing CRM contacts who have started a follow-up sequence but haven't booked a call, sending up to three AI-generated personalized emails every 2 days based on the number of previous follow-ups. When someone books a '30 Minute Meeting' via Calendly, the CRM is updated to reflect that a call is scheduled. Separately, every 6 hours the system checks for prospects marked as 'No' in the 'Showed Call?' column and sends them a re-engagement email.

## Output Details
The workflow outputs updated CRM records in Google Sheets, sends personalized emails via Gmail, and maintains synchronized lead status across the sales pipeline.

## Tags
sales automation, crm, google sheets, gmail, calendly, ai email, follow-up sequence, lead management, no-show recovery
