# Workflow Analysis for Outlook Invoice Automation

## Description
This workflow automates the process of extracting PDF invoices from Outlook emails, uploading them to SharePoint, extracting data from the invoices, and then creating/updating items in a SharePoint list.

## Input Details
The workflow is manually triggered with a "Start" node and uses an Outlook Email node to retrieve emails.

## Process Summary
First, the workflow retrieves emails from Outlook. Next, it checks if the email contains a PDF attachment. If a PDF is found, it is uploaded to a specified SharePoint folder. Subsequently, an AI Builder node is used to extract data from the uploaded PDF invoice. Finally, the extracted data is used to create or update an item in a SharePoint list, with a conditional check to determine whether to create a new item or update an existing one.

## Output Details
The workflow stores extracted invoice data in a SharePoint list, creating new items or updating existing ones as needed.
