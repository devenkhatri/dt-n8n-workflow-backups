# Workflow Analysis for HighLevel Contact Address Verification

## Description
This workflow automatically verifies the mailing address of new contacts added to HighLevel using a third-party address validation service (Lob.com). Based on the verification result, it tags the contact in HighLevel as either 'Mailing Address Deliverable' or 'Mailing Address NOT Deliverable' to support follow-up actions.

## Input Details
The workflow is triggered by a POST webhook from a CRM (like HighLevel) containing contact details including address, city, state, zip code, email, and phone.

## Process Summary
The workflow starts by receiving contact data via a webhook. It then formats the address fields using a Set node. Next, it sends the address details to the Lob.com API for verification. Based on the 'deliverability' response from the API, a Switch node routes the execution: if deliverable, it tags the contact in HighLevel as valid; if not deliverable, it applies a different tag for manual follow-up.

## Output Details
The workflow updates the contact in HighLevel with a tag indicating whether their mailing address is deliverable or not.

## Tags
address verification,HighLevel,CRM integration,webhook,Lob API,contact management,automation
