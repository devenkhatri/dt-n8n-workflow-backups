# Workflow Analysis for InvoiceNinja to Google Sheet Data Logger

## Description
This workflow logs new or updated InvoiceNinja data into a Google Sheet for record-keeping and analysis.

## Input Details
This workflow is triggered by webhooks from InvoiceNinja, receiving data whenever an invoice is created, updated, or deleted.

## Process Summary
The workflow starts by listening for webhook events from InvoiceNinja. When a webhook is received, it processes the incoming data. This data is then formatted and appended as a new row to a specified Google Sheet, effectively recording the InvoiceNinja event.

## Output Details
The workflow outputs the received InvoiceNinja data into a Google Sheet.
