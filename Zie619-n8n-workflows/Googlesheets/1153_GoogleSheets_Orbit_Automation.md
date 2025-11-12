# Workflow Analysis for Moving metrics from Google Sheets to Orbit

## Description
This workflow automates the process of syncing member and activity data from a Google Sheet into the Orbit community management platform, ensuring community metrics are up to date without manual intervention.

## Input Details
The workflow is triggered manually and pulls data from two Google Sheets tabs: 'Members' (containing GitHub usernames and profile info) and 'Activities' (containing associated community activities).

## Process Summary
First, the workflow retrieves member data from the 'Members' tab in Google Sheets. It then uses this data to upsert (create or update) member profiles in Orbit using their GitHub username as the identifier. Simultaneously, it fetches all existing members from Orbit and retrieves related activity records from the 'Activities' tab in Google Sheets. A merge operation links each activity to the corresponding Orbit member using the GitHub username. Finally, the workflow creates or updates activities in Orbit for each matched member.

## Output Details
The workflow outputs updated or newly created member profiles and associated activities in the Orbit workspace, enriching community engagement data.

## Tags
automation, n8n, production-ready, Orbit, Google Sheets, community management, data sync
