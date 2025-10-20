# Workflow Analysis for Pipedrive Won Deal to Stripe Customer and Subscription

## Description
This workflow automates the process of creating a Stripe customer and subscription when a deal is marked as "Won" in Pipedrive.

## Input Details
The workflow is triggered by a "Deal updated" webhook from Pipedrive, specifically when a deal's status changes to "Won".

## Process Summary
The workflow starts by extracting information about the "Won" deal from Pipedrive. It then retrieves the associated person and organization details from Pipedrive. Using this information, it creates a new customer in Stripe. Finally, it creates a new subscription in Stripe for the newly created customer.

## Output Details
The workflow creates a new customer and a new subscription in Stripe.
