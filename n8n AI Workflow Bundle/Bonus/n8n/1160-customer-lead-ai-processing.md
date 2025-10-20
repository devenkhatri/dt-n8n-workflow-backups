# Workflow Analysis for Customer Lead AI Processing

## Description
This workflow processes new customer leads by extracting key information using AI, checking for existing customer records, and then saving the new leads with the extracted data. It can be used by businesses to automate lead qualification and data entry.

## Input Details
This workflow is triggered manually by an HTTP request that provides customer lead data.

## Process Summary
The workflow starts by extracting the customer name and email from the lead data using an AI model. It then checks if a customer with the extracted name already exists. If the customer does not exist, the workflow extracts additional information like the company name, industry, and contact person using another AI model. Finally, it formats the extracted data and saves the new customer lead.

## Output Details
The workflow outputs a success message indicating whether the customer lead was successfully processed and saved.
