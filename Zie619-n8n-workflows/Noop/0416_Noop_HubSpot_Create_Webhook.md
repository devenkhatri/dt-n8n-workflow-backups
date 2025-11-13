# Workflow Analysis for Enrich new Hubspot contacts with contact and company data from ExactBuyer

## Description
This workflow aims to enrich new contacts in HubSpot. The more relevant the HubSpot profile, the more useful it is. Once active, this n8n workflow will update the social profiles, contact data (phone, email) as well as location data from ExactBuyer.

## Input Details
The workflow is triggered when a new contact is created in HubSpot.

## Process Summary
1. The workflow starts when a new contact is created in HubSpot. 2. It then retrieves the full details of the newly created HubSpot contact. 3. Key information like the user ID and email address are extracted from the HubSpot contact data. 4. If an email address is present, the workflow queries the ExactBuyer API to enrich the contact with additional data such as gender, education, location, job title, and company information. 5. Finally, the original HubSpot contact is updated with the comprehensive contact and company data obtained from ExactBuyer.

## Output Details
The workflow updates the existing HubSpot contact with enriched contact and company data from ExactBuyer.

## Tags
HubSpot, ExactBuyer, Contact Enrichment, CRM Automation, automation, n8n
