# Workflow Analysis for Email to Notion Workflow

## Description
This workflow automates the process of saving important emails to a Notion database, extracting key information like sender, subject, and body, and categorizing them for better organization.

## Input Details
This workflow is triggered when new emails are received in a specified Gmail inbox.

## Process Summary
The workflow starts by retrieving new emails from Gmail. It then filters these emails based on specified criteria, such as sender or subject keywords. For each filtered email, relevant data like the sender's email, subject, and body content are extracted. Finally, this extracted information is used to create a new item in a designated Notion database, ensuring that all important email details are systematically recorded.

## Output Details
The workflow creates new pages in a Notion database, containing the sender, subject, and body of relevant emails.
