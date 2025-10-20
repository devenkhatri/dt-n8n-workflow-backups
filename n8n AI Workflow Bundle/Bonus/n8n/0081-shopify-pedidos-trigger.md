# Workflow Analysis for Shopify New Paid Order Webhook and WhatsApp Notification

## Description
This workflow processes new paid orders from Shopify, retrieves product details, transforms the order data, and sends a WhatsApp notification with the order summary.

## Input Details
The workflow is triggered by an HTTP webhook which receives data for new paid orders from Shopify.

## Process Summary
First, the workflow receives new paid order data from Shopify via a webhook. Next, it iterates through the order's line items to retrieve detailed product information from Shopify for each item. Then, it constructs a formatted message containing the customer's name, order ID, and a list of ordered products with their quantities and prices. Finally, the workflow sends this formatted message as a WhatsApp notification.

## Output Details
The workflow sends a WhatsApp message containing details of the new Shopify order.
