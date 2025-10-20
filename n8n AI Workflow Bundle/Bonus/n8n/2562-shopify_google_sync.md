# Workflow Analysis for Shopify and Google Sheets Inventory Sync

## Description
This workflow synchronizes product inventory and order data between Shopify and Google Sheets, allowing for efficient management of product availability and order fulfillment.

## Input Details
The workflow is triggered by new orders in Shopify.

## Process Summary
The workflow starts when a new order is created in Shopify. It then retrieves product information for each item in the order. If the product exists in the Google Sheet database, it updates the "Available" quantity, otherwise, it appends the new product details to the Google Sheet. Finally, it formats the order details and pushes them to a separate "Orders" sheet in Google Sheets.

## Output Details
The workflow updates existing product quantities in Google Sheets, adds new product details if they don't exist, and creates new order entries in a Google Sheet specific for orders.
