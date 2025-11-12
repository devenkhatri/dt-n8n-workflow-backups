# Workflow Analysis for Spot Workplace Discrimination Patterns with AI

## Description
This workflow analyzes employee reviews from Glassdoor to identify potential workplace discrimination patterns across different demographic groups using AI and statistical analysis.

## Input Details
The workflow is triggered manually and receives a company name as input to analyze.

## Process Summary
The workflow starts by scraping Glassdoor reviews for a specified company using ScrapingBee. It extracts overall ratings and demographic-specific review data, then uses AI models to parse this information. Statistical calculations are performed to compute z-scores, effect sizes, and p-values for each demographic group compared to the overall average. Finally, the results are formatted into data visualizations and an AI-generated analysis report.

## Output Details
The workflow produces statistical insights, scatter plots, bar charts, and an AI-generated analysis highlighting potential discrimination patterns in workplace experiences across different demographic groups.

## Tags
workplace discrimination, AI analysis, Glassdoor scraping, demographic analysis, statistical analysis, data visualization, DEI, HR analytics
