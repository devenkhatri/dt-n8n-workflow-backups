# Workflow Analysis for Stripe Payments to Google Sheets and Webhook

## Description
This workflow processes Stripe payments, records new and updated customer information into a Google Sheet, and optionally sends a webhook for successful payments.

## Input Details
The workflow is triggered by webhooks from Stripe, specifically for "checkout.session.completed", "customer.created", and "customer.updated" events.

## Process Summary
The workflow starts by receiving a Stripe webhook. It then checks the event type to determine if it is a checkout session completion, customer creation, or customer update. For checkout session completions, it retrieves customer, payment intent, and product details from Stripe, formats the payment information, and logs it into a designated Google Sheet. For new customers, it adds their details to a Google Sheet. For updated customers, it updates their details in Google Sheets. It then sends an HTTP webhook for successful payments.

## Output Details
The workflow updates and inserts data into a Google Sheet and optionally sends a webhook to a specified URL for successful payments.
