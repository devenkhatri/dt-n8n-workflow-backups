# Workflow Analysis for Set Workflow

## Description
This workflow automatically captures leads from a Typeform submission, formats the data, and creates corresponding records in Pipedrive—including an organization, a contact person, a lead, and a note with additional details.

## Input Details
The workflow is triggered when a user completes a Typeform form, and it receives the form responses including company name, contact name, email, familiarity with n8n, specific questions, and company size (number of employees).

## Process Summary
First, the workflow receives data from a Typeform submission. It then uses a 'Set' node to extract and rename key fields from the form. A function ('Map company size') converts the employee range into a Pipedrive-compatible custom field value. Next, it creates an Organization in Pipedrive with the company name and mapped size. It then creates a Person linked to that organization using the provided name and email. After that, a Lead is created and associated with both the organization and person. Finally, a Note is added to the lead containing the user's questions and original company size.

## Output Details
The workflow outputs structured lead data into Pipedrive by creating an Organization, a Person, a Lead, and a Note—all linked together for sales follow-up.

## Tags
Typeform, Pipedrive, lead generation, form automation, CRM integration, data mapping, n8n
