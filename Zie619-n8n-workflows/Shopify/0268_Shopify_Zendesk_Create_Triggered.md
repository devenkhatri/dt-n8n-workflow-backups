# Workflow Analysis for Set Workflow

## Description
Automated workflow: Set Workflow. This workflow processes data and performs automated tasks.

## Input Details
The workflow is triggered when a customer record is updated in Shopify and receives the updated customer data.

## Process Summary
The workflow is triggered when a customer is updated in Shopify. It searches for the customer in Zendesk by email and extracts their ID, email, and phone number. The Shopify customer data is then merged with the Zendesk user data. If the user exists in Zendesk and their phone number has changed, the contact's phone number is updated in Zendesk. Otherwise, a new contact is created in Zendesk with the customer's details from Shopify.

## Output Details
The workflow either updates an existing contact or creates a new contact in Zendesk.

## Tags
automation, n8n, production-ready, excellent, optimized
