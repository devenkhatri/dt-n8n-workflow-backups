# Workflow Analysis for Stripe Workflow

## Description
This workflow automatically syncs successful Stripe charges to Pipedrive by creating notes on corresponding customer organizations, ensuring sales teams stay updated on payment activity.

## Input Details
The workflow is triggered daily at 8 AM and fetches Stripe charges created since the last execution timestamp.

## Process Summary
The workflow starts by retrieving the last execution timestamp and fetching new successful Stripe charges. It then retrieves customer data from Stripe, renames and filters relevant fields, and merges customer names with charge data. Next, it searches for matching organizations in Pipedrive using the customer name, merges the organization details with the charge data, and creates a note in Pipedrive containing the charge amount, currency, and description linked to the organization. Finally, it updates the last execution timestamp for the next run.

## Output Details
The workflow creates notes in Pipedrive on relevant customer organizations with details of successful Stripe charges.

## Tags
Stripe, Pipedrive, automation, payment sync, CRM integration, daily cron, note creation
