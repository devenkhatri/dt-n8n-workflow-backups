# Workflow Analysis for Pipedrive Dataagma Enrichment

## Description
This workflow enriches Pipedrive contact data using Dataagma, a data enrichment service, to provide more comprehensive contact and organization information.

## Input Details
This workflow is triggered when a new contact is added or updated in Pipedrive.

## Process Summary
The workflow starts by retrieving the new or updated person's data from Pipedrive. It then uses the person's email to query Dataagma for enriched profile information. Next, it extracts the organization's domain from the enriched data and searches for an existing organization in Pipedrive using that domain. If an organization is found, it updates its details with information from Dataagma; otherwise, it creates a new organization. Finally, it updates the person's contact information in Pipedrive, linking them to the enriched organization data.

## Output Details
The workflow updates Pipedrive contacts and organizations with enriched data from Dataagma.
