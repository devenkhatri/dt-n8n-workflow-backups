# Workflow Analysis for Groundhogg CRM Address Verification Workflow

## Description
This workflow automatically verifies the mailing address of new contacts added to Groundhogg CRM using a third-party address validation service (like Lob.com). Based on whether the address is deliverable or not, it tags the contact accordingly in the CRM for follow-up actions.

## Input Details
The workflow is triggered by a POST webhook from Groundhogg CRM containing contact information including address, city, state, and zip code.

## Process Summary
The workflow starts by receiving contact data via a webhook. It then formats the address fields and sends them to an external address verification API. The response includes a 'deliverability' status. Using a switch node, the workflow checks if the address is deliverable. If yes, it tags the contact in Groundhogg as 'Mailing Address Deliverable'; if not, it applies a 'Mailing Address NOT Deliverable' tag to trigger manual review.

## Output Details
The workflow updates the contact record in Groundhogg CRM by applying a tag indicating whether the mailing address is deliverable or not, using HTTP POST requests to the CRM’s API.

## Tags
CRM, address verification, Groundhogg, Lob, webhook, automation, data validation, mailing address, deliverability, contact management
