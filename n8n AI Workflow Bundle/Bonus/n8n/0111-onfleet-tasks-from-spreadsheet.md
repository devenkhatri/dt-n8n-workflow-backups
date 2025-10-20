# Workflow Analysis for Onfleet Task Creation from Spreadsheet

## Description
This workflow automates the creation of tasks in Onfleet using data from a Google Sheet.

## Input Details
This workflow is triggered manually and requires no specific input data upon execution.

## Process Summary
The workflow first reads data from a specified Google Sheet. It then iterates through each row of the spreadsheet data. For each row, it constructs a new task payload for Onfleet, mapping the spreadsheet columns to Onfleet task fields. Finally, it creates a new task in Onfleet with the prepared data.

## Output Details
The workflow creates new tasks in Onfleet based on the data provided in the Google Sheet.
