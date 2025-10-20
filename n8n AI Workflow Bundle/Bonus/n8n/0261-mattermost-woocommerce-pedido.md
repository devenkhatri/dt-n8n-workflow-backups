# Workflow Analysis for WooCommerce New Order Notification to Mattermost

## Description
This workflow automatically sends notifications to a specified Mattermost channel whenever a new order is received in WooCommerce, ensuring that your team is immediately aware of new sales.

## Input Details
The workflow is triggered by an HTTP POST request, likely a webhook from WooCommerce when a new order is placed, and receives order data in its body.

## Process Summary
The workflow starts by receiving an HTTP POST request containing new order details. It then extracts the order ID, status, currency, total amount, and customer email from the received data using a Set node. Finally, it constructs a message with this order information and sends it to a Mattermost channel.

## Output Details
The workflow sends a formatted new order notification to a designated Mattermost channel.
