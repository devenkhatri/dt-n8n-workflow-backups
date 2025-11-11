# Workflow Analysis for Googlesheets Workflow

## Description
This workflow automates sending personalized email sequences to contacts from a Google Sheet, tracks communication status, and sends follow-ups based on predefined timing—while avoiding weekends and preventing duplicate sends.

## Input Details
The workflow is triggered hourly via a schedule trigger and pulls contact and campaign configuration data from a Google Sheet specified in the 'Settings' node.

## Process Summary
First, it checks if it's a weekend and skips execution if so. It loads email campaign settings and contact data from a Google Sheet. For each contact not yet emailed, it prepares and sends the first email. Separately, it checks existing Gmail threads related to the campaign to determine if a follow-up is due based on the days elapsed and message sequence rules. If a follow-up is needed, it prepares and sends the next message in the sequence. All sent emails are tracked by updating the 'first_emailed' column in the Google Sheet.

## Output Details
The workflow sends personalized emails (initial or follow-up) via Gmail and updates the corresponding contact row in the Google Sheet with the date of first contact.

## Tags
email automation, google sheets, gmail, follow-up sequence, scheduled workflow, n8n, no-code automation, lead nurturing, weekend skip, campaign management
