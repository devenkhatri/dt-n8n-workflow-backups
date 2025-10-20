# Workflow Analysis for Shopify Weekly Sales Report to Google Sheets and Email

## Description
This workflow automates the generation of a weekly sales report from Shopify, exports it to a Google Sheet, and sends a notification email with the sheet link.

## Input Details
The workflow is triggered every Monday at 9 AM, initiating the weekly report generation process.

## Process Summary
The workflow starts by setting the date range for the previous week. It then retrieves sales data from Shopify for this period. The aggregated sales data is then appended as a new row to a specified Google Sheet. Finally, an email containing the link to the updated Google Sheet is sent.

## Output Details
The workflow outputs a new row in a specified Google Sheet with the weekly sales data and sends a notification email with a link to this sheet.
