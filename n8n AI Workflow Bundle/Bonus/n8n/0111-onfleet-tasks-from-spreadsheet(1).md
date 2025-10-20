# Workflow Analysis for Onfleet Task Creation from Spreadsheet

## Description
This workflow automates the creation of tasks in Onfleet by reading data from a Google Sheet.

## Input Details
The workflow is triggered manually.

## Process Summary
The workflow starts by manually executing the workflow. Next, it reads data from a specified Google Sheet, extracting information such as recipient name, address, notes, and phone number. Then, it iterates through each row of the spreadsheet data. For each row, it parses the recipient address to retrieve location coordinates. Finally, it creates an Onfleet task using the extracted and processed data.

## Output Details
The workflow creates new tasks in Onfleet.
