# Workflow Analysis for Smartlead Campaign & HubSpot Lifecycle Sync

## Description
This workflow synchronizes campaign data from Smartlead with HubSpot lifecycle stage information, updates PostgreSQL tables with the latest campaign and contact activity, and generates a campaign analytics report in Google Sheets.

## Input Details
The workflow is triggered on a schedule and receives no external input data; it uses configured API keys and environment variables to fetch data from Smartlead and HubSpot.

## Process Summary
The workflow starts by fetching all Smartlead campaigns, then loops through each to extract detailed campaign activity data in CSV format, which is parsed and upserted into a PostgreSQL table. Separately, it queries campaign contacts that need updated HubSpot lifecycle stage info, loops through them, fetches company data from HubSpot, and updates both a HubSpot-specific table and marks the contact as processed. Finally, it aggregates campaign performance metrics from the database and writes them to a Google Sheet for reporting.

## Output Details
The workflow outputs updated records in PostgreSQL tables and a campaign analytics report in a Google Sheet containing metrics like lead counts, opportunity counts, and customer conversions by campaign.

## Tags
campaign sync, Smartlead, HubSpot, PostgreSQL, Google Sheets, automation, reporting, data integration, lifecycle stage, email outreach
