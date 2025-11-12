# Workflow Analysis for Facebook Lead Ads to KlickTipp Integration

## Description
This workflow automatically captures leads from Facebook Lead Ads forms and adds them as subscribers in KlickTipp, mapping form responses to custom fields and enabling instant email campaign triggers.

## Input Details
The workflow is triggered by new form submissions from a specific Facebook Lead Ads form, receiving lead data such as name, email, course selection, payment preference, and comments.

## Process Summary
When a new lead submits a Facebook form, the workflow captures the submission via a webhook. It extracts the first and last name from the full name field. It then maps custom form fields (e.g., course interest, payment method, comments) to corresponding KlickTipp custom fields. Finally, it subscribes the lead to a specified KlickTipp list with the mapped data. Error handling is included to manage potential failures during execution.

## Output Details
The workflow creates or updates a subscriber in KlickTipp with mapped personal and form response data, enabling automated email campaigns based on tags or list membership.

## Tags
Facebook Lead Ads, KlickTipp, lead capture, email marketing, automation, form integration, subscriber management, CRM sync
