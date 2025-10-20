# Workflow Analysis for Form Submission to Pipedrive Deal and Contact Creation

## Description
This workflow automates the process of creating new deals and contacts in Pipedrive whenever a new form submission is received via a webhook. It first checks for an existing person in Pipedrive, creates one if not found, and then creates a new deal linked to that person and organization.

## Input Details
This workflow is triggered by an incoming webhook, receiving data from a form submission.

## Process Summary
The workflow starts by receiving form submission data via a webhook. It then searches for an existing person in Pipedrive using the provided email address. If no person is found, it creates a new person record in Pipedrive. Subsequently, it creates a new organization record in Pipedrive and then creates a new deal, linking it to the newly created or existing person and the new organization.

## Output Details
The workflow creates a new deal and contact (if not existing) in Pipedrive.
