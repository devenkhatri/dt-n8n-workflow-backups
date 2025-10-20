# Workflow Analysis for Airtable to Mailchimp Contact Sync

## Description
This workflow synchronizes contact information from Airtable to Mailchimp, ensuring your mailing list is always up-to-date with your Airtable database.

## Input Details
This workflow is triggered manually.

## Process Summary
The workflow starts by retrieving all records from a specified table in Airtable. It then iterates through each record, extracting the first name, last name, and email address. For each record, it checks if a contact with the extracted email already exists in a specified Mailchimp audience list. Based on whether the contact exists, it either updates the existing Mailchimp contact or creates a new one, subscribing them to the list.

## Output Details
The workflow updates or creates contacts in a specified Mailchimp audience list.
