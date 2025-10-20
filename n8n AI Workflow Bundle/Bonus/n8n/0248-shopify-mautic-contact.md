# Workflow Analysis for Shopify New Customer to Mautic Contact

## Description
This workflow automates the process of adding new Shopify customers as contacts in Mautic, ensuring your marketing platform is always up-to-date with your customer base.

## Input Details
The workflow is triggered by new customer creations in Shopify via a webhook.

## Process Summary
The workflow starts by listening for a new customer creation event from Shopify. It then extracts the customer's first name, last name, and email address. Finally, it creates a new contact in Mautic using the extracted customer information.

## Output Details
The workflow creates a new contact in Mautic with the customer's details.
