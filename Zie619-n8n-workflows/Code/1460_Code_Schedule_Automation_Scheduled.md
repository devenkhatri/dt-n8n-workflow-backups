# Workflow Analysis for INSEE Enrichment for Agile CRM

## Description
This workflow automatically enriches company records in Agile CRM with official French business data from the INSEE OpenData API, including the company’s registered address and SIREN identification number.

## Input Details
The workflow is triggered either manually or on a schedule, and it starts by fetching all company records from Agile CRM.

## Process Summary
The workflow begins by retrieving all company data from Agile CRM. It then filters out any companies marked as read-only using a custom 'RO' field. For the remaining companies, it queries the INSEE API to find matching business records using the company name. Once matched, it merges the CRM data with the INSEE data and updates the CRM record with the official address and SIREN number.

## Output Details
The workflow updates each eligible company record in Agile CRM with enriched data from the INSEE database, specifically the official headquarters address and the SIREN number in custom fields.

## Tags
Agile CRM, INSEE, company enrichment, SIREN, French business data, CRM automation, data enrichment, n8n, production-ready
