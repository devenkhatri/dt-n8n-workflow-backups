# Workflow Analysis for Httprequest Workflow

## Description
This workflow allows users to create a Stripe product and generate a payment link automatically by submitting a simple form with a product title and price.

## Input Details
The workflow is triggered by a form submission that collects a product title (text) and price (number).

## Process Summary
The workflow begins with a form submission that captures a product title and price. It then configures the price in cents and sets the currency to EUR. Next, it creates a new product in Stripe with the provided details. Using the default price from the created product, it generates a Stripe payment link for one quantity of the item. Finally, the workflow redirects the user to a specified URL after successful execution.

## Output Details
The workflow creates a Stripe product and payment link, then redirects the user to a predefined URL.

## Tags
Stripe, payment link, form automation, product creation, n8n, automation, e-commerce
