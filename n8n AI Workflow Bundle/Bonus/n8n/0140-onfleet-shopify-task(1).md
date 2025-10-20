# Workflow Analysis for Shopify Order to Onfleet Task

## Description
This workflow automates the creation of delivery tasks in Onfleet whenever a new paid order is placed in Shopify. It ensures seamless order fulfillment by automatically transferring order details for delivery scheduling.

## Input Details
The workflow is triggered by new paid orders in Shopify via a webhook.

## Process Summary
The workflow starts by retrieving new paid orders from Shopify. It then extracts customer and delivery information from the Shopify order. This data is then used to create a new task in Onfleet, including recipient details and destination. Finally, the workflow logs the successful creation of the Onfleet task.

## Output Details
The workflow creates a new delivery task in Onfleet with details from the Shopify order.
