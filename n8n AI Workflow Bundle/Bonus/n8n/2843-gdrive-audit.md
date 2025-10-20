# Workflow Analysis for Google Drive Audit

## Description
This workflow helps you regularly audit your Google Drive for files that haven't been accessed recently, allowing you to identify and manage potentially outdated or unused content.

## Input Details
This workflow is triggered manually.

## Process Summary
The workflow starts by getting a list of files from a specified Google Drive folder. It then iterates through each file, checking its last accessed time. If a file has not been accessed within the last 90 days, its details are added to a list. Finally, a human-readable table of these inactive files is generated.

## Output Details
The workflow outputs a table of inactive Google Drive files, which can be viewed within n8n.
