# Workflow Analysis for Google Analytics SEO Analysis and Baserow Report

## Description
This workflow automates the process of gathering Google Analytics data, sending it to an AI for SEO analysis, and saving the results to a Baserow database. It compares current week's data with the previous week's data for page engagement, Google Search Console results, and country views.

## Input Details
The workflow is triggered either manually or automatically on a weekly schedule.

## Process Summary
First, the workflow retrieves page engagement statistics, Google Search Console results, and country view data from Google Analytics for both the current and the prior week. Next, custom code nodes parse and transform this raw analytics data into a structured JSON string format. This processed data is then sent to an AI model via HTTP requests, which acts as an SEO expert to compare the two weeks' data and generate SEO improvement suggestions. Finally, the AI's comprehensive analysis and recommendations are stored in a Baserow database.

## Output Details
The workflow produces detailed SEO analysis and actionable suggestions from an AI, which are then stored as new records in a Baserow database.
