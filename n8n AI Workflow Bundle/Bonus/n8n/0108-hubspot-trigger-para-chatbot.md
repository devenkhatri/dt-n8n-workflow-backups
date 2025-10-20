# Workflow Analysis for HubSpot Contact to Chatbot Integration

## Description
This workflow integrates HubSpot contact updates with a chatbot, allowing for personalized interactions based on contact lifecycle stages and other properties.

## Input Details
The workflow is triggered by changes in HubSpot contact properties, specifically when a contact's lifecycle stage is updated or other specified properties change.

## Process Summary
The workflow starts by listening for HubSpot contact updates. It then retrieves additional contact properties from HubSpot based on the updated contact ID. A Set node processes the contact data, followed by an IF node that checks if the contact's lifecycle stage is "customer" or "opportunity". Depending on the lifecycle stage, a separate branch of the workflow is executed, where another IF node further filters based on whether the contact is a "customer". If the contact is a customer, it sends a message via a webhook, including the contact's first name and email.

## Output Details
The workflow sends a personalized message to a chatbot via a webhook if a HubSpot contact is a customer and their lifecycle stage is updated to "customer" or "opportunity".
