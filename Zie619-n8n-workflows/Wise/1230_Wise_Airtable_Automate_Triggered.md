# Workflow Analysis for Wisetrigger Workflow

## Description
Automated workflow: Wisetrigger Workflow. This workflow processes data and performs automated tasks.

## Input Details
This workflow is triggered by a Wise webhook when a transfer state changes and receives data about the transfer.

## Process Summary
The workflow is initiated by a Wise trigger when a transfer's state changes. It then uses the Wise API to fetch full details of the transfer. Subsequently, it extracts and renames key information such as Transfer ID, Date, Reference, and Amount. Finally, this processed transfer data is appended as a new record to "Table 1" in an Airtable base. An error handler is in place to catch any workflow execution errors.

## Output Details
The workflow outputs specific Wise transfer details by appending them as a new record to a specified Airtable base.

## Tags
automation,n8n,production-ready,excellent,optimized
