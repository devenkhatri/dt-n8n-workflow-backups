# Workflow Analysis for Company Data to Airtable

## Description
This workflow automates the process of extracting company data from a website and storing it in an Airtable base. It can be triggered manually and is designed to enrich your CRM or company database with up-to-date information.

## Input Details
This workflow is triggered manually and requires no specific input data to start.

## Process Summary
The workflow starts by retrieving a list of company names from an undefined source. For each company, it then uses the Clearbit API to find detailed company information. This information is then formatted to match the Airtable structure. Finally, it checks if a record for the company already exists in Airtable and either updates the existing record or creates a new one.

## Output Details
The workflow updates or creates company records in a specified Airtable base, enriching it with data from Clearbit.
