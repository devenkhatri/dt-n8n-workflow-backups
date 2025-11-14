# Workflow Analysis for Sync New Shopify Customers to Odoo Contacts

## Description
This workflow automatically synchronizes newly created customer data from Shopify to Odoo, ensuring customer records are consistent across both systems.

## Input Details
This workflow is triggered by new customer creation events in Shopify, receiving customer details such as name, email, and address.

## Process Summary
First, when a new customer is created in Shopify, the workflow searches Odoo to check if a contact with the same email already exists. A code step then processes this search result to determine if the contact is new or existing. Subsequently, a filter node checks this status. If no matching contact is found in Odoo, the workflow proceeds to create a new contact in Odoo using the customer details from Shopify, including their name, email, and primary address information.

## Output Details
The workflow creates a new contact record in Odoo, populating it with the details of the new Shopify customer.

## Tags
Shopify, Odoo, Customer Management, Data Sync, Automation
