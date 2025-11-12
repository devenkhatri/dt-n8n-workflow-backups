# Workflow Analysis for Automate Google Analytics Reporting - AlexK1919

## Description
This workflow automatically pulls Google Analytics data for the current and previous week, including page engagement, Google Search Console metrics, and country-level traffic. It compares the two weeks' data, formats it into a clean HTML report, and emails it to a specified address.

## Input Details
The workflow is triggered manually or via a schedule, and it fetches data from a configured Google Analytics GA4 property using OAuth credentials.

## Process Summary
The workflow first retrieves six sets of data from Google Analytics: page engagement, search console results, and country views for both the current and prior week. Each dataset is parsed and URL-encoded by dedicated code nodes. A 'Set' node compiles these into a single object, which is then aggregated into a structured JSON. Finally, the data is formatted into an HTML report with tables and sent via Gmail.

## Output Details
The workflow produces a formatted HTML email report comparing weekly Google Analytics metrics and sends it to info@alexk1919.com.

## Tags
google analytics, reporting, automation, email report, GA4, weekly report, n8n, production-ready
