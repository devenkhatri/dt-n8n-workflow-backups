# Workflow Analysis for Pipedrive to Stripe Product Synchronization

## Description
This workflow automates the synchronization of products from Pipedrive to Stripe, ensuring that product information is consistent across both platforms.

## Input Details
The workflow is triggered manually and does not receive any external data.

## Process Summary
The workflow starts by retrieving all products from Pipedrive using the Pipedrive CRM node. It then iterates through each Pipedrive product. For every product, it checks if a corresponding product with the same name already exists in Stripe using the Stripe node. If no matching product is found, a new product is created in Stripe with the details from Pipedrive.

## Output Details
The workflow creates new products in Stripe, keeping the Pipedrive and Stripe product lists synchronized.
