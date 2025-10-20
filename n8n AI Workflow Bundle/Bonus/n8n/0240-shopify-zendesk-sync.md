# Workflow Analysis for Shopify Zendesk Customer Sync

## Description
This workflow synchronizes customer data between Shopify and Zendesk, ensuring that customer information is consistent across both platforms. It handles new customer creation in Zendesk if they don't already exist, and updates existing customer information in Zendesk based on Shopify data.

## Input Details
The workflow is triggered by new customer creations or updates in Shopify via a webhook.

## Process Summary
The workflow starts by listening for customer events from Shopify. It then checks if a corresponding user already exists in Zendesk using the customer's email. If the user doesn't exist, a new user is created in Zendesk with the customer's details from Shopify. If the user does exist, their information in Zendesk is updated with the latest customer data from Shopify. Finally, a note is added to the Zendesk user profile indicating the last update time.

## Output Details
The workflow creates new users or updates existing users in Zendesk with Shopify customer data, and adds an internal note to the Zendesk user profile.
