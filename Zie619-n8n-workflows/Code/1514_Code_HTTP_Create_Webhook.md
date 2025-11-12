# Workflow Analysis for Dynamically create tables in Airtable for your Webflow form submissions

## Description
This workflow automatically captures form submissions from a Webflow site and stores them in Airtable. It dynamically creates a new Airtable table for each unique Webflow form (if it doesn't already exist) and logs each submission as a record in the corresponding table. A central index table keeps track of which Webflow form maps to which Airtable table.

## Input Details
The workflow is triggered by a new form submission from a specific Webflow site, receiving the form data including form ID, name, submission timestamp, and field values.

## Process Summary
When a Webflow form is submitted, the workflow first prepares the submission data. It then retrieves the schema of a designated Airtable base to check if a 'Form Index' table exists; if not, it creates one. The workflow searches this index table for an existing entry matching the submitted form ID. If no match is found, it dynamically creates a new Airtable table named after the Webflow form and adds a record to the index table linking the form to its new table. Finally, it inserts the full form submission data as a new record into the appropriate form-specific table in Airtable.

## Output Details
The workflow creates and/or updates tables in an Airtable base: it ensures a 'Form Index' table exists, creates a new table for any previously unseen Webflow form, and adds the form submission as a record in the correct table.

## Tags
Webflow, Airtable, form submissions, dynamic table creation, automation, n8n, production-ready
