# Workflow Analysis for Suspicious Company Domain Alert

## Description
This workflow monitors newly created companies in HubSpot and checks if their domain is suspicious or invalid. If so, it sends an alert to a Slack channel for review.

## Input Details
The workflow is triggered when a new company is created in HubSpot, receiving the company ID as input.

## Process Summary
When a new company is created in HubSpot, the workflow retrieves the company’s details, then attempts to validate its domain by making an HTTP request to a configured base URL (likely an email or domain validation service). If the response status code is not 200 (indicating a problem like a disposable or invalid domain), the workflow sends a formatted alert message to a Slack channel with the company name, domain, and ID.

## Output Details
If a suspicious domain is detected, the workflow posts a warning message to the #hubspot-alerts Slack channel with relevant company details.

## Tags
HubSpot, Slack, domain validation, email verification, automation, alerting, company onboarding
