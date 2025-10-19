# Workflow Analysis for Extract Public Twitter Data from a List of Usernames to CSV

## Description
This workflow is designed to automate the process of gathering public profile information for a list of specified Twitter users, structuring the data, and exporting it into a downloadable CSV file.

## Input Details
The workflow is manually started and uses an internal, hardcoded list of Twitter usernames as its input data source.

## Process Summary
The process begins by reading a static list of Twitter usernames defined within the workflow. It then iterates through each username, using the Twitter API to retrieve detailed public user information. A subsequent step cleans and maps the raw API data, focusing on attributes like name, description, and key public metrics (followers, following, and tweet counts). Finally, all the collected and structured user data is compiled and saved into a single CSV spreadsheet file.

## Output Details
The workflow produces a CSV file named 'TwitterUserList_Data.csv' containing structured public data for all the specified Twitter users.
