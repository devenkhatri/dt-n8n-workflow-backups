# Workflow Analysis for HubSpot Email Follow-up Workflow

## Description
This workflow automates sending follow-up emails via HubSpot when a contact is created or updated, ensuring timely communication and lead nurturing.

## Input Details
The workflow is triggered by an HTTP webhook that receives contact data from HubSpot upon creation or update.

## Process Summary
The workflow starts by receiving contact data from HubSpot. It then checks if the contact has an associated company and if a deal can be found for that company. Depending on whether a deal is found, it sends a follow-up email to the contact using a predefined HubSpot email template. It then logs the email activity in HubSpot.

## Output Details
The workflow sends follow-up emails via HubSpot and creates email engagement records in HubSpot for tracking.
