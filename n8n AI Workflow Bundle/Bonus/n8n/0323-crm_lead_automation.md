# Workflow Analysis for CRM Lead Automation

## Description
This workflow automates the process of managing new leads in a CRM system by classifying them, enriching their data, and creating or updating them in ActiveCampaign based on their classification and existing contact information.

## Input Details
The workflow is triggered manually and requires lead details (email, first name, last name, phone, company, and message) as input.

## Process Summary
The workflow begins by manually receiving lead data. It then classifies the lead using an AI model. Next, it searches for an existing contact in ActiveCampaign using the provided email. Based on whether the lead is classified as "junk" or if an existing contact is found, the workflow either creates a new contact or updates an existing one in ActiveCampaign. If no existing contact is found for a non-junk lead, it enriches the lead data before creating a new contact. Finally, for valid leads, it adds the contact to a specified list in ActiveCampaign.

## Output Details
The workflow creates or updates contact information in ActiveCampaign and adds them to a specific list.
