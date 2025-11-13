# Workflow Analysis for Keap Contact Address Verification Workflow

## Description
This workflow automatically verifies the mailing address of new contacts added to Keap by sending the address details to an external address validation API and then tagging the contact in Keap based on whether the address is deliverable or not.

## Input Details
The workflow is triggered by a webhook from Keap (or another CRM) that sends contact information including address, city, state, and ZIP code.

## Process Summary
The workflow starts when a webhook receives contact data from a CRM. It maps the relevant address fields into a standardized format, then sends those fields to an external address verification API via an HTTP POST request. Based on the API's response, specifically the 'deliverability' field, a Switch node routes the execution: if the address is deliverable, the contact is tagged as verified in Keap; if not, it's tagged for manual review. The workflow uses environment variables for the API URL and webhook endpoint, ensuring flexibility and security.

## Output Details
The workflow updates the contact record in Keap by applying one of two tags: 'Mailing Address Deliverable' or 'Mailing Address NOT Deliverable', enabling downstream automations or manual processes.

## Tags
Keap, address verification, CRM integration, webhook, automation, data validation, contact management
