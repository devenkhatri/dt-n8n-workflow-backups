# Workflow Analysis for CRM Contact Synchronization Workflow

## Description
This workflow synchronizes contact information between two CRM systems (e.g., ActiveCampaign and HubSpot). When a contact is created or updated in the primary CRM, this workflow ensures the information is mirrored in the secondary CRM, and vice-versa, preventing duplicate entries and maintaining data consistency across your platforms.

## Input Details
This workflow is triggered manually and receives contact data as input.

## Process Summary
The workflow starts by retrieving all contacts from ActiveCampaign. It then checks if each contact exists in HubSpot by their email address. If a contact is found in HubSpot, its details are updated; otherwise, a new contact is created. Concurrently, the workflow retrieves all contacts from HubSpot and performs the same check against ActiveCampaign, updating existing contacts or creating new ones as necessary. Finally, it addresses any duplicate contacts by attempting to merge them.

## Output Details
The workflow ensures that contact information is synchronized across both CRM systems, creating or updating contacts as needed, and attempts to merge duplicate contacts in ActiveCampaign.
