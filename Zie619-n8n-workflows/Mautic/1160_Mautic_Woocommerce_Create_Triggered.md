# Workflow Analysis for New WooCommerce Customer to Mautic

## Description
This workflow automates the synchronization of customer data from WooCommerce to Mautic, ensuring customer information is always up-to-date for marketing and CRM purposes.

## Input Details
The workflow is triggered by an event in WooCommerce when a customer is either created or updated, receiving the customer's latest details.

## Process Summary
The workflow initiates upon a customer creation or update event in WooCommerce. It then queries Mautic to check for an existing contact using the customer's email. If no contact is found, a new Mautic contact is created with the customer's details. Conversely, if a contact exists, it is updated with the latest first and last names from WooCommerce. An error handler is included for robust execution.

## Output Details
The workflow either creates a new contact or updates an existing contact in Mautic with the latest customer information from WooCommerce.

## Tags
automation, n8n, production-ready, excellent, optimized
