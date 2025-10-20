# Workflow Analysis for Excel Data to Salesforce Opportunities

## Description
This workflow automates the process of reading data from an Excel file, restructuring it, and creating new opportunities in Salesforce.

## Input Details
The workflow is manually triggered and starts by reading data from an Excel file uploaded to the workflow.

## Process Summary
The workflow begins by reading data from an uploaded Excel file. Next, a Function node processes this data to format dates correctly and maps the Excel column headers to Salesforce field names. Then, the workflow iterates through each reformatted row of data. For each row, it checks if an account already exists in Salesforce based on the "Account Name". If an account exists, its ID is retrieved; otherwise, a new account is created, and its ID is returned. Finally, an opportunity is created in Salesforce using the prepared data and the retrieved or newly created Account ID.

## Output Details
The workflow creates or updates Salesforce Accounts and creates new Salesforce Opportunities based on the Excel file data.
