# Workflow Analysis for Emailreadimap Workflow

## Description
This workflow automatically retrieves emails from a designated 'Invoices' mailbox, extracts their attachments, sanitizes the sender name and date for safe file naming, and saves each attachment to a structured folder in Nextcloud.

## Input Details
The workflow is triggered manually and then automatically fetches emails from an IMAP mailbox named 'Invoices'.

## Process Summary
The workflow starts by reading emails from the 'Invoices' IMAP folder. It then processes each email's attachments using a custom function that sanitizes the filename, sender name, and email date to create safe and organized file paths. Each attachment is converted into a separate item with cleaned metadata. Finally, the workflow uploads each attachment to a Nextcloud folder structured as Documents/Invoices/{date}_{sender}_{filename}.

## Output Details
The workflow saves each email attachment as a file in a designated Nextcloud directory with a standardized, sanitized filename that includes the date and sender.

## Tags
email, imap, nextcloud, file storage, automation, invoice processing, document management
