# Workflow Analysis for Stickynote Workflow

## Description
This workflow automatically processes inbound order emails from Hermas Logistics, extracts key order details like purchase order number, delivery date, and line items, and logs each order line into a Google Sheet for tracking.

## Input Details
The workflow is triggered by a new email in a Gmail inbox, specifically when the email subject contains 'Inbound Order'.

## Process Summary
When a qualifying email arrives, the workflow uses an AI agent (powered by GPT-4o-mini) to parse the email subject and body, extracting the purchase order number, expected delivery date, and list of SKUs with quantities. The AI output is structured into a consistent JSON format. A code node then transforms this data into individual line items, each containing the PO number, delivery date, SKU, and quantity. Finally, each line item is appended as a new row in a designated Google Sheet.

## Output Details
The parsed order line items are stored in a Google Sheet with columns for PO number, expected delivery date, SKU ID, and quantity.

## Tags
automation, email processing, AI parsing, Google Sheets, order management, Gmail trigger, AI agent, structured data extraction
