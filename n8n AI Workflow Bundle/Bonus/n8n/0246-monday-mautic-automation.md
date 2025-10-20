# Workflow Analysis for Monday.com to Mautic Contact Sync

## Description
This workflow automates the synchronization of contact information from Monday.com to Mautic, ensuring that your marketing automation platform always has the most up-to-date lead data from your project management tool.

## Input Details
The workflow is triggered by changes in a Monday.com board, specifically when a new item is created or an existing item is updated, containing relevant contact information.

## Process Summary
First, the workflow receives data from Monday.com about a new or updated item. It then extracts specific fields like name, email, and phone number from the Monday.com item. Next, it searches Mautic to see if a contact with the extracted email already exists. If the contact exists, the workflow updates their details in Mautic; otherwise, it creates a new contact in Mautic with the provided information. Finally, it ensures that Monday.com and Mautic have consistent contact data.

## Output Details
The workflow updates existing contacts or creates new contacts in Mautic based on the information received from Monday.com.
