# Workflow Analysis for AI Company Researcher for Sales

## Description
This workflow automates the research of companies using AI to generate sales outreach messages and update a CRM.

## Input Details
The workflow is manually triggered and uses predefined company names as input.

## Process Summary
First, the workflow iteratively processes a list of company names. For each company, it uses an AI model to research the company and extract relevant information for sales. Then, it uses another AI model to craft a personalized sales outreach message based on the gathered information. Finally, it checks if the company already exists in HubSpot and creates or updates the company and a associated deal with the generated sales message.

## Output Details
The workflow updates HubSpot CRM with company information, creates or updates deals, and includes personalized sales outreach messages.
