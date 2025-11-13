# Workflow Analysis for Formtrigger Workflow

## Description
This workflow automates the process of capturing leads through a web form, verifying their email addresses, enriching their data with person and company information, and then adding them as leads to HubSpot.

## Input Details
This workflow is triggered by an n8n form submission that captures a business email address.

## Process Summary
First, the workflow verifies the submitted business email using Hunter.io. If the email is valid, it proceeds to enrich the person's data (e.g., name, job title) and the associated company's data (e.g., company name, size) using Clearbit. Finally, the enriched lead information is added to HubSpot. If the email is not valid, the workflow concludes without further action.

## Output Details
The workflow produces a new lead entry in HubSpot with enriched person and company data.

## Tags
automation,n8n,production-ready,excellent,optimized,lead capture,email verification,data enrichment,CRM,HubSpot
