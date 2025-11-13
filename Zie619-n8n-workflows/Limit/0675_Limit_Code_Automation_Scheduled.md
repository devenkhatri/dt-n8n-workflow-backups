# Workflow Analysis for Scheduled Strava Activity Sync to Google Sheets

## Description
This workflow automatically synchronizes new Strava activities to a Google Sheet, ensuring that all recent activities are recorded and duplicates are avoided.

## Input Details
The workflow is triggered automatically every two hours and receives recent activity data from Strava, along with previously recorded activity IDs from a Google Sheet.

## Process Summary
The workflow starts by fetching the latest activities from Strava and simultaneously retrieves the IDs of activities already saved in a Google Sheet. It then uses a code node to filter out any Strava activities that have already been recorded. The newly identified activities are formatted to extract relevant details like distance, date, time, and elevation. Finally, these new and formatted activities are appended as new rows to a designated Google Sheet.

## Output Details
The workflow appends new Strava activity data, including distance, unique reference ID, date, track URL, time, and elevation, to a Google Sheet named "n8n" in the "Sherlo_Bike" document.

## Tags
Strava, Google Sheets, Data Sync, Automation, Scheduled, Activity Tracking
