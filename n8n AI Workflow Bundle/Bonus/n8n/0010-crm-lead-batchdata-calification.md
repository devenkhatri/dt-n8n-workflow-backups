# Workflow Analysis for CRM Lead Batch Data Qualification

## Description
This workflow automates the process of qualifying leads from a CSV file by enriching their data, assessing their sentiment, and categorizing them using AI. It helps businesses process large batches of leads efficiently and makes lead qualification faster and more consistent.

## Input Details
This workflow is manually triggered and processes lead data from a user-uploaded CSV file.

## Process Summary
The workflow starts by reading lead data from a CSV file. It then iteratively processes each lead, enriching contact and company information using Hunter.io and Clearbit, respectively. Next, it analyzes the sentiment of the lead's description using an AI model and classifies the lead into predefined categories. Finally, it formats the processed lead data, including the enriched information, sentiment, and classification, for output.

## Output Details
The workflow outputs a CSV file containing the original lead data augmented with enriched contact details, company information, sentiment analysis results, and AI-based lead categorization.
