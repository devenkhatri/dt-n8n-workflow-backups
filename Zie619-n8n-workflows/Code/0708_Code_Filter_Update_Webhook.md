# Workflow Analysis for LinkedIn Profile Enrichment Workflow

## Description
This workflow automatically enriches LinkedIn profile data by fetching detailed information from RapidAPI and updating a Google Sheet with the results, saving time for recruiters, sales, and marketing teams.

## Input Details
The workflow is manually triggered and pulls LinkedIn profile URLs from a specified Google Sheet.

## Process Summary
The workflow starts by reading LinkedIn URLs from a Google Sheet. It filters out profiles that have already been enriched. For the remaining profiles, it encodes the URL and calls the RapidAPI Fresh LinkedIn Profile Data endpoint to retrieve detailed profile information. It then processes the API response to remove array fields and preserves the original row number. Finally, it updates the Google Sheet by appending or updating the enriched profile data using the LinkedIn URL as the matching key.

## Output Details
The workflow updates the original Google Sheet with enriched LinkedIn profile data, including fields like about, job title, company info, contact details, and more.

## Tags
linkedin, enrichment, rapidapi, google sheets, automation, lead generation, talent sourcing, n8n
