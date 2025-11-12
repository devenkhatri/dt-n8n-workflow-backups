# Workflow Analysis for Streamline data from an n8n form into Google Sheet and Airtable

## Description
This workflow collects user data through an n8n form, processes it to extract and format submission date and time, saves the data to both Google Sheets and Airtable, and sends two confirmation emails to the user.

## Input Details
The workflow is triggered by form submissions from an n8n form that collects the user's name, city, and email address.

## Process Summary
When a form is submitted, the workflow first extracts the submission timestamp and splits it into separate Date and Time fields. It then reformats the input fields into standardized column names (Name, City, Email, Date, Time). The formatted data is simultaneously written to a Google Sheet and an Airtable base. Finally, two customized confirmation emails are sent to the user's email address—one with a static subject and another that includes the submission date in the subject line.

## Output Details
The workflow appends the processed data to a Google Sheet, creates a new record in Airtable, and sends two confirmation emails to the form submitter.

## Tags
form automation, Google Sheets, Airtable, email notification, data processing, n8n workflow, production-ready
