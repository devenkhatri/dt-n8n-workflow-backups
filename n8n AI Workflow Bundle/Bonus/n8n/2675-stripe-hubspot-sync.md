# Workflow Analysis for Stripe to HubSpot Customer Sync

## Description
This workflow automatically syncs customer data from Stripe to HubSpot, ensuring your CRM is always up-to-date with your latest customer information from your payment gateway.

## Input Details
The workflow is triggered by an HTTP webhook, typically set up to receive events from Stripe when a new customer is created or updated.

## Process Summary
The workflow starts by receiving customer data from a Stripe webhook. It then processes this data, extracting relevant customer fields and preparing them for HubSpot. Next, it checks if a contact with the given email already exists in HubSpot. If the contact exists, it updates their information; otherwise, it creates a new contact. Finally, the workflow adds the contact to a specified HubSpot list based on whether the contact was updated or newly created.

## Output Details
The workflow updates or creates contact records in HubSpot and adds them to a designated marketing list.
