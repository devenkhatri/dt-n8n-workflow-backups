# Workflow Analysis for UTM Link Creator & QR Code Generator with Scheduled Google Analytics Reports

## Description
This workflow automates the creation of marketing links with UTM tracking parameters, stores them in a database, generates QR codes for offline use, and sends scheduled Google Analytics performance reports to the marketing team.

## Input Details
The workflow is triggered manually for UTM link creation (with required campaign parameters) and on a schedule for Google Analytics reporting.

## Process Summary
First, the workflow accepts UTM campaign parameters like source, medium, and campaign name, then constructs a full tracking URL using those parameters. It saves this UTM link to an Airtable database for record-keeping and generates a QR code by making an HTTP request to a QR generation service. Separately, on a schedule, it fetches Google Analytics data (e.g., sessions by source/medium) and uses an AI agent to create an executive summary. Finally, this summary is emailed to the marketing manager.

## Output Details
The workflow outputs a UTM-tracked URL saved in Airtable, a QR code generated via HTTP request, and a scheduled email report with Google Analytics insights sent to the marketing manager.

## Tags
UTM, QR code, Google Analytics, marketing automation, Airtable, scheduled reporting, campaign tracking, n8n
