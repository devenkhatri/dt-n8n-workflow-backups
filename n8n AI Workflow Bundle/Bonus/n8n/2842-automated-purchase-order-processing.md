# Workflow Analysis for Automated Purchase Order Processing with OpenAI GPT-4

## Description
This workflow automates the processing of purchase order emails. It extracts key information from PDF attachments using AI, verifies the vendor, creates a draft purchase order in QuickBooks, and sends a confirmation email.

## Input Details
The workflow is triggered manually by a user, but it is designed to process email attachments containing purchase orders.

## Process Summary
The workflow starts by retrieving attachment data. It then uses OpenAI GPT-4 to extract purchase order information from the PDF. The extracted vendor name is used to search for the corresponding vendor in QuickBooks. If a vendor is found, a draft purchase order is created in QuickBooks. Finally, a confirmation email with the extracted purchase order details is sent.

## Output Details
The workflow creates a draft purchase order in QuickBooks and sends a confirmation email to a specified address.
