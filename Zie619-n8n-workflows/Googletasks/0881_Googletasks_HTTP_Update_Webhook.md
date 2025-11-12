# Workflow Analysis for EU Legislative Sustainability Tracker

## Description
This workflow automatically scrapes EU legislative procedures scheduled for debate yesterday, uses an AI model to identify which ones are related to sustainability, and then records those relevant procedures in a Google Sheet while creating follow-up Google Tasks for review.

## Input Details
The workflow is triggered manually and begins by fetching HTML data from a configured EU legislative webpage via an HTTP request.

## Process Summary
First, the workflow fetches and parses HTML blocks from a legislative webpage to extract details like reference number, committee, rapporteur, title, and PDF link. It then loops through each legislative item and sends the title and committee info to an AI (OpenAI) to classify whether the item is sustainability-related. The AI's 'yes'/'no' response is captured, and only items marked 'yes' pass through an If condition. These sustainability-related items are then written to a Google Sheet and used to create individual Google Tasks for follow-up study.

## Output Details
The workflow outputs sustainability-related EU legislative records to a Google Sheet and creates corresponding Google Tasks for scheduled review.

## Tags
EU legislation, sustainability, AI classification, web scraping, Google Sheets, Google Tasks, automation, n8n
