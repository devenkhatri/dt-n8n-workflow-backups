# Workflow Analysis for HubSpot to Zendesk Company Sync

## Description
This workflow synchronizes company information from HubSpot to Zendesk, ensuring that company records are consistent across both platforms. It handles both new company creation and updates to existing company details based on changes in HubSpot.

## Input Details
The workflow is triggered manually and does not receive any external data.

## Process Summary
The workflow starts by retrieving all companies from HubSpot. For each HubSpot company, it checks if a corresponding organization exists in Zendesk. If not, it creates a new organization in Zendesk using data from HubSpot. If an organization already exists, it updates the Zendesk organization with any changed company details from HubSpot, ensuring that both systems reflect the latest information.

## Output Details
The workflow creates new organizations or updates existing organizations in Zendesk based on HubSpot company data.
