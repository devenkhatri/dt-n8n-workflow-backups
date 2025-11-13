# Workflow Analysis for Stripe Payment Order Sync – Auto Retrieve Customer & Product Purchased

## Description
Automated workflow: Stripe Payment Order Sync – Auto Retrieve Customer & Product Purchased. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered by a Stripe webhook when a checkout session is completed, receiving payment event data.

## Process Summary
The workflow initiates when a Stripe checkout session is successfully completed. It then makes an HTTP request to retrieve detailed session information, specifically expanding the line items to get product details. Finally, it extracts and sets key information such as the customer's name, email, and the description of the purchased product.

## Output Details
The workflow prepares structured customer and product purchase information for subsequent use, but does not explicitly send it to an external system within this configuration.

## Tags
automation,n8n,production-ready,excellent,optimized
