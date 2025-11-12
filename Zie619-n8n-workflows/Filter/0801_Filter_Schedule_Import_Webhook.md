# Workflow Analysis for Shopify Fulfillment Automation

## Description
This workflow automates the fulfillment of unfulfilled Shopify orders by retrieving fulfillment order IDs and marking them as fulfilled, ideal for stores selling digital products or using automated fulfillment services.

## Input Details
The workflow is triggered either manually (via 'Test workflow' button) or on a schedule, and begins by fetching unfulfilled orders from a Shopify store using configured credentials.

## Process Summary
First, the workflow sets a store ID variable and retrieves all unfulfilled Shopify orders. It then filters orders that are older than 24 hours. Using a loop mechanism, it processes each order to fetch its associated fulfillment orders via the Shopify API. Finally, it creates a fulfillment request for each valid order, notifying the customer upon completion.

## Output Details
The workflow sends POST requests to Shopify’s fulfillment API to mark orders as fulfilled and optionally notifies customers, completing the automated fulfillment process.

## Tags
Shopify, fulfillment automation, e-commerce, digital products, order processing, n8n, API integration, scheduled automation
