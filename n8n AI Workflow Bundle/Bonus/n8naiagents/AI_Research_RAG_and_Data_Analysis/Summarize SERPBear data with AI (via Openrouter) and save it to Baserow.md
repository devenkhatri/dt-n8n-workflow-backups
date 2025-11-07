# Workflow Analysis for Automated SERPBear Keyword Ranking Analysis with AI and Baserow

## Description
This workflow automates the process of fetching keyword ranking data from SERPBear, uses AI to analyze the performance and trends, and then saves the detailed analysis into a Baserow database for easy tracking and reporting.

## Input Details
The workflow is triggered either manually or on a weekly schedule, initiating the process of fetching keyword data for analysis.

## Process Summary
First, the workflow fetches keyword ranking data for a specific domain from a SERPBear instance. Next, it processes this raw data to calculate current positions, 7-day average positions, and identify ranking trends (improving, declining, stable) for each keyword. This processed data is then formatted into a detailed prompt and sent to an AI model for comprehensive analysis. Finally, the AI-generated analysis, along with the current date and blog name, is saved as a new record in a Baserow database.

## Output Details
The workflow outputs a structured AI analysis of SEO keyword rankings, which is then stored as a new record in a Baserow database.
