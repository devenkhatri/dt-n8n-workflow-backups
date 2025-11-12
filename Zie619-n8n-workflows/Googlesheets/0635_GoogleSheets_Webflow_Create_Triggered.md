# Workflow Analysis for Code Workflow

## Description
This workflow automatically captures form submissions from a Webflow site and appends the data—including a timestamp—to a Google Sheet, enabling seamless lead or message tracking without manual intervention.

## Input Details
The workflow is triggered by a form submission on a Webflow site, receiving the form payload and submission timestamp via a Webflow webhook.

## Process Summary
When a form is submitted on Webflow, the workflow captures the payload data and submission date. A code node extracts the form fields and adds the submission date as a new field. The processed data is then formatted to match the target Google Sheet columns. Finally, the workflow appends this enriched data as a new row in the specified Google Sheet, automatically creating columns if needed.

## Output Details
The workflow appends a new row containing the form data and submission date to a designated Google Sheet.

## Tags
Webflow, Google Sheets, form automation, data logging, no-code automation, n8n
