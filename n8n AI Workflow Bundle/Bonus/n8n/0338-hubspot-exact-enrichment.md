# Workflow Analysis for HubSpot Contact Enrichment with Exact Data

## Description
This workflow enriches HubSpot contact data using Exact's API, fetching additional contact information and updating HubSpot accordingly. It's designed to keep your CRM data comprehensive and up-to-date, providing your sales and marketing teams with more complete prospect and customer profiles. This automation is particularly useful for businesses that rely on accurate and detailed contact information for personalized outreach and segmentation.

## Input Details
This workflow is manually triggered or can be configured to run on a schedule to enrich HubSpot contact data.

## Process Summary
The workflow starts by retrieving all companies associated with "Contact" from HubSpot. For each company, it then searches for contacts within that company. If contacts are found, it queries Exact for the email address with information obtained from HubSpot. Finally, it updates the "Exact Contact Enrichment" property in HubSpot with the retrieved Exact contact details.

## Output Details
The workflow updates the "Exact Contact Enrichment" property of HubSpot contacts with data from Exact, providing enriched contact profiles.
