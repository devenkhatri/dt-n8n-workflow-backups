# Workflow Analysis for Spot Workplace Discrimination Patterns with AI

## Description
This workflow analyzes employee reviews from Glassdoor to detect potential workplace discrimination patterns across different demographic groups using AI and statistical analysis.

## Input Details
The workflow is triggered manually and starts with a predefined company name (e.g., 'Twilio') to analyze.

## Process Summary
The workflow begins by scraping Glassdoor reviews for a specified company using ScrapingBee. It extracts overall review statistics and demographic-specific ratings from the page content. Using these data points, it calculates statistical measures like variance, standard deviation, z-scores, effect sizes, and p-scores to identify significant disparities in employee experiences across different demographic groups. Finally, it formats the results into visual charts and generates an AI-powered analysis summarizing key findings about potential discrimination patterns.

## Output Details
The workflow produces data visualizations (scatterplot and bar chart) via QuickChart and generates an AI-written analysis highlighting discrimination patterns and employee experience insights.

## Tags
workplace discrimination, AI analysis, Glassdoor scraping, demographic analysis, statistical analysis, z-score, effect size, data visualization, employee reviews, diversity and inclusion
