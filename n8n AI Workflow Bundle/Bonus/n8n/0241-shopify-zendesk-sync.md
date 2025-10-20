# Workflow Analysis for Shopify Zendesk Customer Sync

## Description
This workflow synchronizes customer data between Shopify and Zendesk, ensuring that customer information is consistent across both platforms. When a new customer is created or an existing customer is updated in Shopify, the workflow checks if a corresponding user exists in Zendesk. If not, a new user is created in Zendesk. If a user already exists, their information is updated to reflect the changes in Shopify.

## Input Details
This workflow is triggered by webhooks from Shopify whenever a new customer is created or an existing customer is updated.

## Process Summary
The workflow starts by receiving customer data from Shopify. It then searches for a user in Zendesk using the provided email address. Based on whether a user is found, it either creates a new user in Zendesk or updates an existing one, ensuring that the Zendesk user profile matches the Shopify customer data.

## Output Details
The workflow creates new users or updates existing user profiles in Zendesk based on Shopify customer data.
