# Workflow Analysis for Itemlists Workflow

## Description
This workflow processes sample contact data from a FileMaker database, extracts individual contact records, and returns the field data for each contact.

## Input Details
The workflow is triggered manually and does not receive external input data.

## Process Summary
The workflow starts with a manual trigger. It then uses a function node to generate sample FileMaker contact data containing 100 records. An ItemLists node splits the response.data array into individual items. Finally, a FunctionItem node extracts and returns the fieldData from each contact record.

## Output Details
The workflow outputs the fieldData of each contact record, which includes personal and contact information like name, address, phone numbers, email, and company details.

## Tags
automation, n8n, production-ready, excellent, optimized, filemaker, data-processing, contact-data
