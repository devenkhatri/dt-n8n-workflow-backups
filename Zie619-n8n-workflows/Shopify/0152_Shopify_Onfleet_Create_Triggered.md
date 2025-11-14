# Workflow Analysis for Creating an Onfleet Task for a new Shopify Fulfillment

## Description
This workflow automates the creation of delivery tasks in Onfleet whenever a new fulfillment order is generated in Shopify, streamlining the delivery process.

## Input Details
The workflow is triggered by a Shopify webhook whenever a new fulfillment is created in Shopify.

## Process Summary
1. The workflow starts when a new fulfillment is created in Shopify.
2. It then proceeds to create a new task in Onfleet using the information from the Shopify fulfillment.
3. In case of an error during the process, the workflow stops and logs an error.

## Output Details
The workflow creates a new delivery task in Onfleet.

## Tags
automation, n8n, production-ready, excellent, optimized
