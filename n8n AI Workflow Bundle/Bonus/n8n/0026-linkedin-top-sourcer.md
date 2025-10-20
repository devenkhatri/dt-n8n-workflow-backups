# Workflow Analysis for LinkedIn Top Sourcer Workflow

## Description
This workflow helps recruiters and sourcers efficiently find prime candidates on LinkedIn by automating profile data extraction and enrichment using AI.

## Input Details
The workflow is manually triggered by the user and starts by asking for a LinkedIn URL to begin the sourcing process.

## Process Summary
First, the workflow extracts the plain text content from the provided LinkedIn profile URL. Next, it uses a large language model to extract specific candidate information like name, current role, company, contact details, and skills from the extracted text. Then, it constructs a Google search query to find the candidate's email address. Finally, it attempts to verify the found email address and enriches the candidate data with an AI-generated summary.

## Output Details
The workflow compiles a comprehensive candidate profile including AI-enriched data, email verification status, and a summarized overview, which can then be used for outreach or record-keeping.
