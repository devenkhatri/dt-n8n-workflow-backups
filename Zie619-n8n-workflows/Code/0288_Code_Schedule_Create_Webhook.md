# Workflow Analysis for Sync Stripe Charges to HubSpot Contacts

## Description
This workflow automatically syncs payment data from Stripe to HubSpot by aggregating total charges per customer and updating their contact record in HubSpot with the total spend.

## Input Details
The workflow is triggered on a daily schedule and fetches all charges from Stripe via the Stripe API.

## Process Summary
The workflow starts by fetching all charges from Stripe. It filters out charges without a customer, removes duplicate customer entries to avoid redundant API calls, and retrieves detailed customer data from Stripe. It then merges charge and customer data, aggregates the total amount captured per customer email, and updates or creates the corresponding HubSpot contact with the total spend in USD. Optionally, it creates a custom HubSpot contact property if it doesn't already exist.

## Output Details
The workflow updates or creates contacts in HubSpot with a custom property showing their total spend from Stripe charges.

## Tags
Stripe, HubSpot, customer sync, payment data, automation, scheduled workflow, data aggregation, CRM integration
