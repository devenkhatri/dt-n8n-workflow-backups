# Workflow Analysis for Typeform to Pipedrive Integration

## Description
This workflow automates the process of capturing Typeform submissions and updating or creating leads in Pipedrive. It streamlines lead management by automatically populating Pipedrive with information from new Typeform entries.

## Input Details
The workflow is triggered by new Typeform submissions via a webhook.

## Process Summary
The workflow starts by receiving a new Typeform submission. It then retrieves the answers from the form, extracts the email to search for an existing person in Pipedrive, and creates a new organization and person in Pipedrive if they don't already exist. Finally, it creates a new deal in Pipedrive, linking it to the newly created or existing person and organization.

## Output Details
The workflow creates or updates persons, organizations, and deals in Pipedrive based on the Typeform submission data.
