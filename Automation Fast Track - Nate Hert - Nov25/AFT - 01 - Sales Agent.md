# Workflow Analysis for Sales Agent Workflow

## Description
This comprehensive workflow automates lead management, sales follow-ups, meeting scheduling, and no-show reminders. It integrates with Google Sheets for lead and CRM data, uses AI for personalized email generation, and tracks meeting schedules via Calendly.

## Input Details
The workflow is triggered by scheduled intervals for lead processing, scheduled intervals for follow-up emails, a Calendly event for new invitees, and scheduled intervals for identifying no-show contacts.

## Process Summary
This workflow runs in four distinct flows. First, it regularly fetches new leads from a Google Sheet, transfers them to a CRM Google Sheet, and removes them from the source. Second, it periodically identifies contacts in the CRM needing follow-ups, generates personalized emails using AI based on the follow-up stage, sends these emails via Gmail, and updates the CRM. Third, it detects new "30 Minute Meeting" bookings in Calendly and updates the "Call Scheduled?" status in the CRM. Finally, it regularly checks for "no-show" contacts in the CRM, sends them a rescheduling email via Gmail, and updates their status.

## Output Details
The workflow produces personalized follow-up emails, no-show reminder emails, and updates Google Sheets (lead list and CRM) with lead information, follow-up statuses, and call scheduling details.
