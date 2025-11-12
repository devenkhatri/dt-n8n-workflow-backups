# Workflow Analysis for Google Keep Notes to Google Sheets Exporter

## Description
This workflow automatically exports Google Keep notes from a specified Google Drive folder, filters and processes them (optionally using AI), and saves selected note details into a Google Sheet.

## Input Details
The workflow is triggered manually and receives JSON files from a designated Google Drive folder that contains exported Google Keep notes.

## Process Summary
The workflow starts by manually triggering a search in a specific Google Drive folder for files. It processes files in batches of 10, downloads only JSON files, and parses their content. It filters out archived notes and optionally applies AI processing to extract specific information (like expense amounts). Finally, it formats key note fields (text, creation/edit dates, archive status, and extracted data) and appends them to a Google Sheet.

## Output Details
The workflow outputs processed Google Keep note data into a specified Google Sheet, including note content, timestamps, archive status, and any AI-extracted values like expense amounts.

## Tags
Google Keep, Google Drive, Google Sheets, AI processing, JSON parsing, expense tracking, automation, note export, data migration, n8n
