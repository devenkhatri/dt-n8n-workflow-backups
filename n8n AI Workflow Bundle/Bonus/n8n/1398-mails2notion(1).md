# Workflow Analysis for Email to Notion Database

## Description
This workflow automates the process of saving incoming emails to a Notion database, extracting key information like sender, subject, and content.

## Input Details
The workflow is triggered by new emails received in a specified inbox.

## Process Summary
The workflow starts by retrieving new emails. For each email, it extracts the sender's email, subject, and plain text content. It then creates a new item in a specified Notion database, mapping the extracted email details to corresponding Notion properties like "From", "Subject", and "Content".

## Output Details
The workflow creates new items in a Notion database, each representing an email with its relevant details.
