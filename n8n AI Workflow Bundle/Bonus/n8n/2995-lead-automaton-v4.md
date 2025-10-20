# Workflow Analysis for Lead Automaton

## Description
This workflow automates the process of identifying potential leads from a list of websites, enriching their data, and organizing them for outreach.

## Input Details
This workflow is manually triggered and processes a list of website URLs for lead generation.

## Process Summary
The workflow starts by extracting the base domain from each provided URL. It then uses the Clearbit API to enrich the company data associated with each domain. Subsequently, it searches for key contact persons within these companies using another Clearbit API call. Finally, it formats the collected company and person data into a structured output, ready for export or further processing.

## Output Details
The workflow outputs a collection of enriched company and contact person data, providing details like company name, website, social links, and contact information for potential leads.
