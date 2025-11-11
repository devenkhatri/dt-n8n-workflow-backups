# Workflow Analysis for Low Stock & Sold Out Watcher for Shopify

## Description
This workflow monitors Shopify inventory levels in real time and sends alerts via Discord when a product is running low (less than 4 units) or is completely out of stock. It uses Shopify webhooks to trigger checks, fetches detailed product info via GraphQL, and sends rich, formatted messages with product images and inventory details.

## Input Details
The workflow is triggered by a Shopify webhook that sends a POST request containing inventory level update data (available quantity and inventory item ID).

## Process Summary
1. A webhook receives inventory update data from Shopify. 2. A code node evaluates whether the item is low in stock (<4 units) or out of stock (0 units). 3. Conditional 'IF' nodes route the data based on inventory status. 4. For each case, a GraphQL query fetches detailed product information including title, variant, image, and current inventory. 5. An HTTP request sends a customized Discord message with product details and appropriate alert color (yellow for low stock, red for out of stock).

## Output Details
The workflow sends formatted Discord messages to designated channels notifying the team about low stock or out-of-stock products, including product images, titles, variants, and inventory levels.

## Tags
Shopify, inventory management, Discord, webhook, GraphQL, low stock alert, out of stock alert, automation, e-commerce
