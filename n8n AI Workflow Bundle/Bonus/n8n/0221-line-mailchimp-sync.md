# Workflow Analysis for LINE to Mailchimp Contact Sync

## Description
This workflow automates the synchronization of new contacts from LINE to Mailchimp, ensuring your email marketing lists are always up-to-date with your LINE audience.

## Input Details
The workflow is triggered by an HTTP Webhook, expecting contact data from a LINE messaging platform.

## Process Summary
The workflow starts by receiving contact data via an HTTP Webhook. It then extracts the user's name and LINE user ID from the received data. Next, it modifies the extracted name to ensure it's in a suitable format for Mailchimp, combining first and last names if available. Finally, it adds or updates this contact in a specified Mailchimp audience, mapping the LINE user ID to a custom merge field and adding the contact to a "LINE Contacts" tag.

## Output Details
The workflow updates or adds contact information, including name, email, and LINE user ID, to a specified Mailchimp audience and tags them accordingly.
