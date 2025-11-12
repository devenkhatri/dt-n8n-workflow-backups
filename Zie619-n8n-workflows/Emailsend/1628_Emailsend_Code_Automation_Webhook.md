# Workflow Analysis for Property Lead Contact Enrichment from CRM

## Description
This workflow automates the process of finding high-potential real estate investment leads by searching for properties that match specific criteria, enriching them with owner contact details, scoring them based on investment potential, and delivering the results via Excel, CRM, and email.

## Input Details
The workflow is triggered either manually or on a daily schedule and starts with predefined property search criteria such as location, price range, equity, and ownership status.

## Process Summary
The workflow begins by configuring search parameters for properties in Austin, TX, then calls a property search API to retrieve matching listings. It filters these results using custom logic to identify high-value leads—such as absentee owners with long ownership tenure and no recent sales—and assigns each a lead score. For each qualified property, it fetches owner contact information via a skip-tracing API, formats all data into a standardized lead record, and then outputs the results in three ways: saving to an Excel file, pushing to HubSpot CRM, and sending an email notification with a summary and attachment.

## Output Details
The workflow produces a scored list of enriched real estate leads, saves them as an Excel file, adds them to HubSpot CRM, and sends a summary email with the file attached.

## Tags
real estate, lead generation, property search, skip trace, CRM integration, automation, n8n, Excel export, email notification, HubSpot
