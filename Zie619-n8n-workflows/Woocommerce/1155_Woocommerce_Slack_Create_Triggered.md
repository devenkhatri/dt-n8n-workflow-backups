# Workflow Analysis for New WooCommerce refund to Slack

## Description
This workflow automatically monitors WooCommerce orders and notifies a Slack channel if a significant refund is issued.

## Input Details
This workflow is triggered by an "order updated" event in WooCommerce, receiving the updated order data.

## Process Summary
First, the workflow is activated when an order is updated in WooCommerce. It then checks if the updated order has a "refunded" status and if its total amount is 100 or more. If both conditions are met, a custom message is prepared. Finally, this message, containing details about the refunded order, is sent to a specified Slack channel.

## Output Details
The workflow sends a detailed notification about the significant refunded order to a designated Slack channel.

## Tags
automation, n8n, production-ready, excellent, optimized
