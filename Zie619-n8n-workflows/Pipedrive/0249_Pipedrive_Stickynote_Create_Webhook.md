# Workflow Analysis for Production Workflow

## Description
When a new organization is created in Pipedrive, the workflow enriches the company data via Datagma, extracts employee information, filters for ideal buyer leads, finds their email addresses, adds those people to Pipedrive and updates the organization with enriched details.

## Input Details
Triggered by a Pipedrive webhook when a new organization is added, receiving the organization’s meta data.

## Process Summary
1) The trigger captures the new organization and passes its name to a Datagma HTTP request that returns full and premium company data including employees. 2) The employee list is split into individual items. 3) Each employee is evaluated; if their score exceeds 0.1 and their job title contains “sales”, they are considered an ideal buyer. 4) For ideal buyers, another Datagma request fetches their email address, the data is prepared and merged with the original employee record. 5) The merged record is used to create a new person in Pipedrive and to update the organization’s custom fields with funding, traffic, industry, website, employee count, and address.

## Output Details
Creates new person records in Pipedrive for ideal buyers and updates the organization’s custom properties with enriched company information.

## Tags
Pipedrive,Datagma,lead enrichment,webhook,automation,organization,person,ideal buyer
