# Workflow Analysis for Automated Online Marketing Report Generation

## Description
This workflow automates the generation and delivery of daily, weekly, or monthly online marketing reports using data from Google Analytics and Google Ads, distributed via email and Google Drive.

## Input Details
The workflow is triggered manually or on a preset schedule (daily, weekly, or monthly).

## Process Summary
First, the workflow clears any existing data in a Google Sheet, then retrieves data from Google Analytics and Google Ads, processing each data source sequentially. It then appends this new marketing data to the Google Sheet. Finally, the workflow generates a Google Document report from a template, converts it to PDF, shares it via email, and uploads it to Google Drive.

## Output Details
The workflow produces a PDF marketing report, which is sent via email and uploaded to Google Drive.
