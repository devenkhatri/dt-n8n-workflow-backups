# Workflow Analysis for AFT - 03 - Onboarding Agent

## Description
This workflow automates the client onboarding process by generating contracts when deals are marked as closed, monitoring for signed contracts to send welcome emails, and creating shared Google Drive folders when onboarding calls are booked.

## Input Details
The workflow is triggered by changes in a Google Sheet (when 'Closed?' column is updated), hourly schedule triggers, and Calendly event bookings for onboarding calls.

## Process Summary
When a deal is marked closed in Google Sheets, the system fetches sales transcripts from Fathom, extracts contract details using AI, and creates a PandaDoc contract. It then updates the sheet and emails a team member to review the contract. Separately, the system checks hourly for newly signed contracts and sends a welcome email to the client. Additionally, when a client books an onboarding call via Calendly, a Google Drive folder is created and shared with them.

## Output Details
The workflow produces PandaDoc contracts, updates the Google Sheet with contract status, sends internal review emails, client welcome emails, and creates/shared Google Drive folders for new clients.

## Tags
onboarding, contract generation, PandaDoc, Google Sheets, Calendly, Google Drive, AI extraction, client management, automation
