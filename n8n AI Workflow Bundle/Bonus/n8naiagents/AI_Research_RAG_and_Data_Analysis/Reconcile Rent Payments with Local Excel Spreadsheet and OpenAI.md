# Workflow Analysis for AI-Powered Bank Statement Reconciliation for Rental Payments

## Description
This workflow automates the reconciliation of bank statements with rental payments by using an AI agent to identify discrepancies and actions required for tenants. It interacts with a local Excel spreadsheet for tenant and property details, ensuring data privacy.

## Input Details
The workflow is triggered automatically when a new CSV bank statement file is added to a specified local folder.

## Process Summary
The workflow first reads the newly added CSV bank statement and extracts its data. It then utilizes an AI agent, powered by an OpenAI chat model, to analyze this bank statement data against tenant and property information retrieved from a local Excel spreadsheet. The AI agent identifies issues such as missed or incorrect rental payments, expiring tenancies, and outstanding fees. Finally, the identified actions and discrepancies are formatted and appended as new rows to an "alerts" sheet within the same local Excel spreadsheet.

## Output Details
The workflow updates a local Excel spreadsheet by appending a detailed report of identified actions and discrepancies related to rental payments.
