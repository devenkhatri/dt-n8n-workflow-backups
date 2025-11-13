# Workflow Analysis for Shopify + Mautic

## Description
Automated workflow: Shopify + Mautic. This workflow integrates 10 different services: webhook, stickyNote, mautic, graphql, set. It contains 28 nodes and follows best practices for error handling and security.

## Input Details
This workflow is triggered by Shopify customer updates and by incoming webhooks from Mautic.

## Process Summary
This workflow handles two main events. First, when a customer is updated in Shopify, it searches for the contact in Mautic. If the contact exists, it updates their Mautic segment based on their Shopify email marketing consent (subscribed or unsubscribed). If the contact does not exist in Mautic, it creates a new one and then updates their Mautic segment based on Shopify consent. Second, when a Mautic webhook is received and validated, it queries Shopify for the customer by email. If the customer is found, it updates their Shopify email marketing consent based on the Mautic subscription status (contactable or not).

## Output Details
The workflow updates customer segments in Mautic, creates new Mautic contacts, and updates customer email marketing consent in Shopify.

## Tags
automation,n8n,production-ready,excellent,optimized
