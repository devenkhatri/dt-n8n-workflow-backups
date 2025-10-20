# Workflow Analysis for Webflow Form Submission to Discord and Google Sheets

## Description
This workflow automates the processing of new form submissions from Webflow. It sends notifications to a Discord channel and records the submission details in a Google Sheet. If a file is uploaded, the workflow also uploads it to Google Drive before sending the Discord notification.

## Input Details
The workflow is triggered by new form submissions from a Webflow form, receiving the submission data and form name.

## Process Summary
First, the workflow checks if a file was uploaded with the form submission. If a file exists, it is uploaded to Google Drive. Next, a Discord notification is sent, including details from the Webflow form and a link to the uploaded file if applicable. Finally, the form submission data, along with Google Drive file IDs and links if present, is appended as a new row in a specified Google Sheet.

## Output Details
The workflow sends a Discord notification to a specified channel and appends a new row with form submission data to a Google Sheet, potentially including Google Drive file details.
