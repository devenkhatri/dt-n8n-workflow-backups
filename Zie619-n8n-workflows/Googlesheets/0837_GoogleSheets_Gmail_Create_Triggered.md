# Workflow Analysis for Googledrive Workflow

## Description
This workflow automatically processes emails with attachments from a specific Gmail label, verifies if the sender is on a whitelist in Google Sheets, and organizes the attachments in Google Drive by company and month.

## Input Details
The workflow is triggered by new emails in Gmail that match a specific label (Label_2), and it receives email data including sender, date, and attachments.

## Process Summary
The workflow starts by polling Gmail for new emails with a specific label. It then looks up the sender's email in a Google Sheet whitelist to get the associated company name. It checks if a company-specific folder exists in Google Drive under a parent 'Invoices' folder, creating it if necessary. Next, it checks for a YYYY/MM subfolder within the company folder and creates it if missing. The email attachments are split into individual files, each prefixed with a timestamp, and uploaded to the appropriate YYYY/MM folder in Drive.

## Output Details
The workflow uploads email attachments to a structured Google Drive folder hierarchy organized by company name and year/month, with metadata such as sender email and date embedded in the file properties.

## Tags
Google Drive, Gmail, Google Sheets, file automation, email processing, folder organization, whitelist filtering, attachment handling
