# Workflow Analysis for Receive a Mattermost message when new data gets added to Airtable

## Description
This workflow automatically notifies users on Mattermost when new data is added to an Airtable base, ensuring timely communication about new entries.

## Input Details
The workflow is triggered every minute by new data added to the "Data" table in Airtable, specifically monitoring the "Created" field.

## Process Summary
First, the workflow is activated when new data is detected in a specified Airtable table. Next, it extracts the ID and Name from the newly added record in Airtable. Finally, it constructs a message using this information. This message is then sent to a designated channel in Mattermost.

## Output Details
The workflow sends a formatted message containing the ID and Name of the new Airtable record to a specified Mattermost channel.

## Tags
automation,n8n,production-ready,excellent,optimized
