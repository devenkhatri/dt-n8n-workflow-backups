# Workflow Analysis for Automated Lead Alert System

## Description
This workflow automates the process of notifying sales teams about new leads and updating a CRM (Leadlovers) with their details. It ensures no lead goes unnoticed and streamlines lead management.

## Input Details
This workflow is triggered manually and does not receive any input data.

## Process Summary
The workflow starts by retrieving new leads from a Google Sheet. For each lead, it checks if a unique identifier exists to avoid duplicates. If the lead is new, it adds the lead to an internal n8n database and then updates the lead in Leadlovers CRM. Finally, it sends a notification via Telegram alerting the sales team about the new lead.

## Output Details
The workflow updates the Leadlovers CRM with new lead information and sends a Telegram message to the sales team with lead details.
