# Workflow Analysis for Google Analytics SEO Report to AI and Baserow

## Description
This workflow automates the analysis of Google Analytics data, comparing current week's performance with the previous week for page engagement, Google Search Console results, and country-specific views. It leverages AI to generate SEO insights and suggestions.

## Input Details
The workflow is triggered either manually or on a weekly schedule, and it fetches Google Analytics data as its primary input.

## Process Summary
The workflow first retrieves page engagement statistics, Google Search Console results, and country view data for the current week and the prior week from Google Analytics. This raw data is then processed and transformed by code nodes into a URL-encoded JSON format. Subsequently, this processed data is sent to an AI model via HTTP requests, which acts as an SEO expert to compare the two weeks' data and generate 5 SEO improvement suggestions. Finally, the AI's detailed analysis and suggestions are stored in a Baserow database.

## Output Details
The workflow produces AI-generated SEO reports, including comparative data tables and actionable suggestions, which are then saved into a Baserow database.
