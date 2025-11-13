# Workflow Analysis for Stickynote Workflow

## Description
This workflow automates the lead qualification and management process by capturing form submissions, verifying email addresses, enriching contact data, and then creating or updating records in Pipedrive CRM.

## Input Details
The workflow is triggered by an n8n form submission, receiving a business email address.

## Process Summary
1. A business email is collected via an n8n form.
2. The email address is verified for validity using Hunter.io. If invalid, the process stops.
3. If valid, Clearbit enriches the contact details based on the email.
4. The workflow searches Pipedrive for the person and their organization. If either is new, they are created in Pipedrive.
5. Finally, a new lead is created in Pipedrive, associated with the person and organization.

## Output Details
The workflow populates a Pipedrive CRM with new or updated person and organization records, and creates a new lead.

## Tags
automation, n8n, production-ready, excellent, optimized
