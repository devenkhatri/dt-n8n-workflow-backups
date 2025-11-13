# Workflow Analysis for Production Workflow

## Description
This workflow generates product label data by combining product, fabric, and roll information from multiple databases for printing purposes.

## Input Details
The workflow is triggered by a POST webhook request containing product grade ID, movement detail ID, and an array of fabric roll IDs.

## Process Summary
The workflow starts by receiving product and roll data via a webhook. It fetches printing configuration settings from an external HTTP service. Then it queries MySQL to get detailed product information including fabric width and composition using the provided product grade ID. Simultaneously, it extracts roll IDs and queries a PostgreSQL database for roll-specific details. Finally, it merges the product and roll data using the movement detail ID as the key.

## Output Details
The workflow outputs merged product and roll data ready for label printing, though the final destination (e.g., API response, file, or printing system) is not explicitly defined in the provided nodes.

## Tags
label printing, product data, MySQL, PostgreSQL, webhook, data merge, fabric composition, manufacturing, inventory management
