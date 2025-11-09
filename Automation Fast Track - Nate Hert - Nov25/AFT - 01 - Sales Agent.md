# Workflow Analysis for AFT - 01 - Sales Agent

## Description
An automated sales workflow that moves new leads from a list into a CRM, sends up to three AI-personalized follow-up emails every two days, updates CRM records when calls are scheduled via Calendly, and follows up with no-shows.

## Input Details
The workflow is triggered by scheduled intervals to check for new leads, existing CRM entries for follow-ups, and Calendly booking events; it receives lead data from Google Sheets and event data from Calendly.

## Process Summary
First, new leads from a Google Sheet are transferred to a CRM sheet, assigned unique IDs, and removed from the original list. Separately, the system checks CRM records every few days to identify leads eligible for follow-up emails (based on last contact date and number of prior follow-ups), generates personalized messages using AI, sends them via Gmail, and updates follow-up status. When a Calendly '30 Minute Meeting' is booked, the CRM is updated to mark the lead as having scheduled a call. Additionally, leads manually marked as 'No' in the 'Showed Call?' column are automatically emailed a no-show follow-up and their status is updated.

## Output Details
The workflow outputs updated CRM records in Google Sheets, sends personalized follow-up and no-show emails via Gmail, and deletes processed leads from the original list.

## Tags
sales automation, CRM sync, email follow-up, lead management, Calendly integration, Google Sheets, AI personalization, no-show recovery
