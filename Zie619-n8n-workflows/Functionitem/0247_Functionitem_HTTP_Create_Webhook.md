# Workflow Analysis for Pipedrive Product to Stripe Sync

## Description
This workflow automatically creates a product in Stripe whenever a new product is added in Pipedrive, and then sets up corresponding price records in Stripe based on the pricing data from Pipedrive.

## Input Details
The workflow is triggered by a new product creation event in Pipedrive and receives the product data including name, description, and pricing information.

## Process Summary
When a new product is created in Pipedrive, the workflow captures the product details and sends a request to Stripe to create a corresponding product. It then extracts the newly created Stripe product ID and combines it with the original product data. Next, it splits out each price entry (if multiple exist) and creates individual price records in Stripe linked to the new product ID, converting the price into cents as required by Stripe's API.

## Output Details
The workflow creates a product and one or more associated price records in Stripe, ensuring product data is synchronized from Pipedrive to Stripe.

## Tags
Pipedrive, Stripe, product sync, automation, e-commerce, API integration
