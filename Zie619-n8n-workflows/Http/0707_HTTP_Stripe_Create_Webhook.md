# Workflow Analysis for Sync Stripe Payments to QuickBooks

## Description
This workflow automatically syncs successful Stripe payments to QuickBooks by creating or updating customer records and posting sales receipts.

## Input Details
The workflow is triggered by a Stripe 'payment_intent.succeeded' webhook event containing payment and customer details.

## Process Summary
When a successful Stripe payment is detected, the workflow retrieves the associated Stripe customer data. It then checks if the customer already exists in QuickBooks by querying customer records. If the customer exists, it proceeds to create a sales receipt in QuickBooks using the existing customer reference. If not, it creates a new QuickBooks customer using Stripe customer details before creating the sales receipt. The payment, customer, and receipt data are merged at key steps to ensure accurate record linkage.

## Output Details
The workflow creates a sales receipt in QuickBooks Online linked to an existing or newly created customer, with details from the Stripe payment.

## Tags
Stripe, QuickBooks, payment sync, automation, accounting, webhook, sales receipt, customer sync
