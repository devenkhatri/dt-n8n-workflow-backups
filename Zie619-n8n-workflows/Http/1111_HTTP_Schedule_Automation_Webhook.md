# Workflow Analysis for Automating Betting Data Retrieval with TheOddsAPI and Airtable

## Description
This workflow automatically fetches betting data for ice hockey (or other sports) twice daily—once in the morning to get upcoming events and again at night to retrieve final scores—and stores or updates the information in an Airtable database.

## Input Details
The workflow is triggered on a schedule: once at 7:00 AM to fetch upcoming events and again at 11:00 PM to fetch event results, using TheOddsAPI.

## Process Summary
At 7:00 AM, the workflow calls TheOddsAPI to retrieve upcoming ice hockey events and creates new records in Airtable with event details like teams, start time, and sport info. At 11:00 PM, it fetches the day's final scores and results from the same API. It then merges this score data with the previously stored upcoming events by matching event IDs. Finally, it updates the corresponding Airtable records with the scores, completion status, and last update timestamp.

## Output Details
The workflow creates and updates records in an Airtable base with betting-related event data, including upcoming games in the morning and final scores at night.

## Tags
betting, sports data, automation, TheOddsAPI, Airtable, scheduled workflow, ice hockey, data sync, n8n
