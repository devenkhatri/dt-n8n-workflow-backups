# Workflow Analysis for Production Workflow

## Description
This workflow automatically retrieves a list of workflows from an n8n instance, processes the data, and uploads the result as a JSON file to a specified Google Drive folder. It runs daily at 2:30 AM and includes error handling for robust execution.

## Input Details
The workflow is triggered either manually or automatically via a cron job set to run daily at 2:30 AM.

## Process Summary
The workflow starts by fetching a list of workflows from the n8n API using basic authentication. It then maps the response data into individual items for processing. Separately, it also fetches detailed data for a specific workflow. These data streams are merged by index, transformed into binary JSON format, and prepared for upload. Finally, the resulting JSON file is uploaded to a designated Google Drive folder.

## Output Details
The workflow produces a JSON file containing workflow data and uploads it to a specified folder in Google Drive.

## Tags
automation, n8n, production-ready, Google Drive, cron, API integration, error handling
