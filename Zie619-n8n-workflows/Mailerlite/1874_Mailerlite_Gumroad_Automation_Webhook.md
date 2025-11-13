# Workflow Analysis for Gumroad Sale Trigger

## Description
This workflow automates customer management and record-keeping in response to new sales on Gumroad, integrating with MailerLite for email marketing and Google Sheets for CRM.

## Input Details
The workflow is triggered by a new sale event from Gumroad, receiving details about the purchased product and customer information via a webhook.

## Process Summary
When a new Gumroad sale occurs, the workflow first adds the buyer's email and country as a new subscriber in MailerLite. Subsequently, it assigns this subscriber to a specific group in MailerLite via an HTTP request. Concurrently, it appends a new row to a Google Sheets CRM, recording the sale timestamp, product name, customer email, and country.

## Output Details
The workflow adds a new subscriber and assigns them to a group in MailerLite, and updates a Google Sheets CRM with new sale records.

## Tags
Gumroad, MailerLite, Google Sheets, CRM, Sales Automation, Email Marketing, Data Management
