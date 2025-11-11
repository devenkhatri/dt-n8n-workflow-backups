# Workflow Analysis for Postgrestrigger Workflow

## Description
This workflow automatically captures user updates from a Postgres database, filters out internal n8n.io email addresses, and saves qualified leads to a Google Sheet for follow-up.

## Input Details
The workflow is triggered by an UPDATE event on the 'users' table in a Postgres database, though currently the trigger is disabled and testing uses manual input with mock data.

## Process Summary
The workflow starts by listening for updates to the 'users' table in Postgres (currently disabled). For testing, a manual trigger provides mock user data. A filter node excludes any records with 'n8n.io' in the email field. The remaining qualified user data is then sent to a Google Sheet named 'Qualified leads to contact', where it is appended or updated based on the user ID. Error handling is included to manage failures during execution.

## Output Details
Qualified user records (excluding n8n.io emails) are saved or updated in a specified Google Sheet under the 'Sheet1' tab.

## Tags
Postgres, Google Sheets, lead sync, data filtering, automation, n8n, production-ready
