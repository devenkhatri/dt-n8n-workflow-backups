# Workflow Analysis for Automated SEO Audit Report Generator

## Description
This workflow automates the generation of SEO audit reports for a given website URL. It leverages various SEO tools to gather data, analyzes it with AI, and then compiles a comprehensive report and sends it via email.

## Input Details
The workflow is manually triggered and takes a website URL as input.

## Process Summary
The workflow starts by retrieving the sitemap from the provided URL. It then fetches website data and analyzes it using an AI model to identify SEO issues and generate recommendations. Subsequently, it retrieves SEO data from Google Search Console and Lighthouse, and combines all the collected data. Finally, it formats the data into a comprehensive report.

## Output Details
The workflow generates a detailed SEO audit report and sends it to a specified email address.
