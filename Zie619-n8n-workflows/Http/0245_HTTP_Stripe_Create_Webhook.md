# Workflow Analysis for If Workflow

## Description
This workflow monitors Pipedrive deals for updates, and when a deal's 'won time' changes, it retrieves the associated organization's details, checks if the organization exists as a customer in Stripe, and creates a new Stripe customer if it doesn't exist.

## Input Details
The workflow is triggered by an update to a deal in Pipedrive and receives the updated deal data including current and previous states.

## Process Summary
The workflow starts when a Pipedrive deal is updated. It checks if the 'won_time' field has changed. If so, it fetches the associated organization's details from Pipedrive. It then queries an external API (likely Stripe) to search for an existing customer with the organization's name. If no matching customer is found, it proceeds to create a new customer in Stripe using the organization's address and name information.

## Output Details
If the organization doesn't already exist as a customer, the workflow creates a new customer record in Stripe with the organization's details.

## Tags
Pipedrive, Stripe, deal won, customer creation, automation, CRM, payment
