# Workflow Analysis for UTM Link Creator & QR Code Generator with Scheduled Google Analytics Reports

## Description
This workflow automates the creation of marketing links with UTM tracking parameters, stores them in a database, generates QR codes for offline use, and sends scheduled Google Analytics performance reports to the marketing manager.

## Input Details
The workflow is triggered manually to create UTM links (with required parameters like URL, campaign source, medium, etc.) and on a schedule to fetch and email Google Analytics reports.

## Process Summary
First, the workflow accepts UTM parameter inputs and constructs a tracked URL by appending those parameters. It then saves this UTM link to an Airtable database for record-keeping. Simultaneously, it generates a QR code for the UTM link using an HTTP request to a QR generation service. Separately, on a schedule, it pulls session and source/medium data from Google Analytics, uses an AI agent to analyze the data and create an executive summary, and emails that summary to the marketing manager.

## Output Details
The workflow outputs a UTM-tracked URL stored in Airtable, a corresponding QR code generated via HTTP request, and scheduled email reports with AI-summarized Google Analytics insights sent to the marketing manager.

## Tags
UTM, QR code, Google Analytics, marketing automation, Airtable, scheduled reports, link tracking, n8n, production-ready
