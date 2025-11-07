# Workflow Analysis for Umami Analytics to AI and Baserow Report

## Description
This workflow automates the process of extracting website analytics from Umami, analyzing the data using an AI model, and then saving the generated insights into a Baserow database for reporting and content optimization.

## Input Details
The workflow is initiated either manually by clicking "Test workflow" or automatically via a weekly schedule every Thursday, and subsequently retrieves data from Umami Analytics.

## Process Summary
The workflow begins by fetching overall website view statistics for the last 7 days from Umami, which are then processed and sent to an AI model for a summary analysis. Subsequently, it retrieves page-specific metrics for both the current and previous week from Umami, processes this data, and sends it to the AI for a comparative analysis and SEO improvement suggestions. Finally, the AI-generated summaries and suggestions are prepared for storage.

## Output Details
The workflow outputs the AI-generated summary of overall view stats, the AI-generated comparison of page data with improvement suggestions, and the current date, which are all stored as new records in a specified Baserow table.
