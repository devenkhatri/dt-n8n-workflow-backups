# Workflow Analysis for Sync New Shopify Products to Odoo Product

## Description
This workflow automates the synchronization of new product listings from Shopify to Odoo. It ensures that products created in Shopify are automatically added to Odoo, streamlining product data management between the two platforms.

## Input Details
The workflow is triggered by new product creation events in Shopify and receives product data directly from Shopify's webhook.

## Process Summary
1. The workflow is initiated when a new product is created in Shopify.
2. It then queries Odoo to check for the existence of a product with a matching product ID.
3. A code node processes the Shopify product data and the Odoo query result to determine if the product is new to Odoo.
4. If the product does not exist in Odoo, an Odoo node creates a new product record.
5. The Odoo product is populated with details such as name, product ID, description, and list price from the Shopify product data.

## Output Details
The workflow creates new product records in Odoo based on new product creations in Shopify.

## Tags
automation, n8n, production-ready, excellent, optimized, Shopify, Odoo, Product Sync, Integration
