# Workflow Analysis for ERP Lead Automation

## Description
This workflow automates the process of creating and updating leads in an ERP system, enriching lead data, and managing communication and task creation based on lead status.

## Input Details
The workflow is triggered manually and requires input lead data.

## Process Summary
The workflow starts by retrieving lead information from a Google Sheet. It then processes each lead individually, checking if the lead already exists in Zoho CRM. If a lead exists, it updates the existing lead in Zoho CRM; otherwise, it creates a new lead. It further enriches lead data using the Hunter.io API. Finally, based on the lead status, it creates tasks, sends emails, or makes API calls to other systems.

## Output Details
The workflow updates or creates leads in Zoho CRM, creates tasks, sends emails, and interacts with other APIs based on lead status.
