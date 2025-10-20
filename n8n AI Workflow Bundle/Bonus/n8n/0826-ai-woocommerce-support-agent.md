# Workflow Analysis for AI WooCommerce Support Agent

## Description
This workflow uses AI to act as a support agent for your WooCommerce store by answering customer questions and managing orders.

## Input Details
This workflow is triggered manually and receives customer questions and order details as input.

## Process Summary
The workflow starts by extracting the customer's question and checking if it's an order-related query. If it is, the workflow retrieves order information from WooCommerce. It then uses an AI model (OpenAI's ChatGPT) to generate an answer to the customer's question, leveraging either the retrieved order data or general product information. Finally, it sends the AI-generated response back to the customer.

## Output Details
The workflow sends an AI-generated response to the customer, addressing their query.
