# Workflow Analysis for Airtable Workflow

## Description
This workflow retrieves contact data from Airtable and adds them as leads to a Lemlist email outreach campaign, then verifies if the lead was successfully created.

## Input Details
The workflow is manually triggered and does not receive external input data.

## Process Summary
The workflow starts with a manual trigger. It then fetches records from an Airtable base. For each record, it creates a lead in Lemlist using the email and name from Airtable, associating it with a specific campaign. After creation, it attempts to retrieve the same lead from Lemlist to confirm successful addition. If any step fails, the workflow stops with an error message.

## Output Details
The workflow outputs confirmation of lead creation in Lemlist and halts with an error message if any operation fails.

## Tags
automation, airtable, lemlist, lead generation, email outreach, manual trigger, production-ready
