# Workflow Analysis for Create Custom Presentations per Lead

## Description
This workflow automatically creates personalized Google Slides presentations for each lead by pulling lead data from uploaded CSV or Excel files, storing it in a newly created Google Sheet, and replacing placeholders in a presentation template with the lead's details.

## Input Details
The workflow is triggered when a new file (CSV or Excel) is added to a specific Google Drive folder, and it receives the file metadata including its ID and MIME type.

## Process Summary
The workflow starts by detecting a new file in a designated Google Drive folder. It checks the file type and extracts lead data if it's a CSV or Excel file. A new Google Sheet is created with the current date, and the lead data is appended to it. Then, for each lead, the workflow copies a presentation template, replaces placeholders like company name and contact name with actual lead data, and moves the new Google Sheet to a specific folder. Finally, it updates the sheet with the corresponding presentation ID.

## Output Details
The workflow produces customized Google Slides presentations for each lead and updates a Google Sheet with the presentation IDs, storing both in specified Google Drive folders.

## Tags
automation, google drive, google sheets, google slides, lead management, presentation automation, csv processing, excel processing, template customization, n8n
