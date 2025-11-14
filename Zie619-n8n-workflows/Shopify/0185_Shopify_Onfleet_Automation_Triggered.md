# Workflow Analysis for Updating Shopify tags on Onfleet events

## Description
Automated workflow: Updating Shopify tags on Onfleet events. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered by an Onfleet webhook when an Onfleet task is delayed.

## Process Summary
The workflow starts when a task in Onfleet is delayed. It then connects to Shopify to perform an update operation. Specifically, it updates the tags for a Shopify item. If any errors occur during this process, an error handler will stop the workflow execution.

## Output Details
The workflow updates the tags of an item in Shopify.

## Tags
automation,n8n,production-ready,excellent,optimized
