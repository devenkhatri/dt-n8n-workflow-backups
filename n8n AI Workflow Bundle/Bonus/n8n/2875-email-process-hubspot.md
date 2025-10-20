# Workflow Analysis for Automated Email Processing and HubSpot Contact Management

## Description
This workflow automates the processing of incoming emails, extracts key information, and either updates existing HubSpot contacts or creates new ones based on the email content.

## Input Details
The workflow is triggered by new emails received in a specific inbox.

## Process Summary
The workflow starts by retrieving new emails and extracting relevant information like sender email, subject, and body. It then searches HubSpot for an existing contact using the sender's email. If a contact exists, the workflow updates their information with the details from the email. If no contact is found, a new HubSpot contact is created using the extracted email data.

## Output Details
The workflow updates existing HubSpot contacts or creates new ones based on the processed email information.
