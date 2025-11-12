# Workflow Analysis for If Workflow

## Description
This workflow automatically enriches and syncs lead and company data from ConvertKit form subscriptions to HubSpot, using Clearbit for data enrichment. It filters out personal email addresses and only processes business emails, ensuring that contacts and their associated companies are properly created or updated in the CRM.

## Input Details
The workflow is triggered when a user subscribes to a specific ConvertKit form, providing subscriber email data.

## Process Summary
The workflow starts when someone subscribes to a ConvertKit form. It first filters out personal email domains to only process business emails. It then uses Clearbit to enrich the subscriber's email, retrieving personal and company details. If a company domain is found, it searches for the company in HubSpot. If the company doesn't exist, it creates a new company record with enriched data; if it does exist, it updates the company with the latest information. Finally, it upserts the contact in HubSpot and associates them with the company.

## Output Details
The workflow creates or updates company and contact records in HubSpot CRM with enriched data from Clearbit, ensuring business leads are properly tracked and associated.

## Tags
automation, lead enrichment, CRM sync, HubSpot, Clearbit, ConvertKit, email filtering, company data, contact management
