# Workflow Analysis for New WooCommerce order to Slack

## Description
This automated workflow detects new orders in WooCommerce and processes the order details. It is optimized for production use with comprehensive error handling, security, and documentation.

## Input Details
The workflow is triggered by the creation of a new order in WooCommerce and receives all associated order data.

## Process Summary
When a new order is created in WooCommerce, the workflow first checks if the total order price is greater than or equal to 100. If this condition is met, it then sends a notification message to a designated Slack channel, including details such as order ID, status, total, and a link to the order. An error handler is in place for any workflow execution issues.

## Output Details
The workflow sends a formatted message containing new order details to the "woo-commerce" channel in Slack.

## Tags
automation,n8n,production-ready,excellent,optimized
