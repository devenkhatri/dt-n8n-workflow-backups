# Workflow Analysis for MySQL Workflow for Missing Project Costs

## Description
This workflow automates the process of identifying active projects in a MySQL database that are missing budgeted cost information and then sends email notifications to relevant cost center teams.

## Input Details
The workflow is triggered weekly at 8 AM by a schedule trigger and does not receive external data.

## Process Summary
The workflow initiates weekly to query a MySQL database for open, external, and active projects that have a zero budgeted cost. It then groups these projects by company and cost center, counting the number of projects for each. Based on the identified cost center, the workflow routes the information and sends an automated HTML email to a specific recipient, notifying them about the number of active projects with missing budgeted costs for that cost center and requesting coordination with the Accounts Team for updates.

## Output Details
The workflow sends HTML emails to a specified recipient (amjid@amjidali.com) with details about projects missing budgeted costs, categorized by their respective cost centers.

## Tags
automation, n8n, production-ready, excellent, optimized, mysql, email, reporting, cost management, project management
