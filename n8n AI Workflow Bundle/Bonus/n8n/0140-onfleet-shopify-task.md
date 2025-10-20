# Workflow Analysis for Onfleet Shopify Task Creation

## Description
This workflow automates the creation of delivery tasks in Onfleet based on new orders from Shopify. It retrieves order details, extracts relevant shipping information, and then creates a task in Onfleet for delivery.

## Input Details
The workflow is triggered manually and does not receive any input data.

## Process Summary
The workflow starts by retrieving a specific Shopify order using its ID. It then extracts the customer's shipping address, including the full address, zip, city, country, and province. This extracted address is then used to create a new delivery task in Onfleet. Finally, it retrieves and outputs the created task from Onfleet.

## Output Details
The workflow outputs the details of the newly created Onfleet task.
