# Workflow Analysis for Onfleet to QuickBooks Invoice Creation

## Description
This workflow automates the creation of QuickBooks invoices from Onfleet task data, ensuring accurate and timely billing for services rendered.

## Input Details
The workflow is triggered manually.

## Process Summary
The workflow starts by retrieving Onfleet tasks. It then identifies unique recipient names from these tasks. For each unique recipient, it aggregates the relevant task data. Finally, it creates an invoice in QuickBooks for each recipient using the aggregated task information.

## Output Details
The workflow creates invoices in QuickBooks based on Onfleet task data.
