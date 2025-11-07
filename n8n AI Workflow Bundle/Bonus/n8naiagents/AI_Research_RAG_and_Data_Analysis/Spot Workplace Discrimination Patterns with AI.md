# Workflow Analysis for Spot Workplace Discrimination Patterns with AI

## Description
This workflow analyzes Glassdoor reviews to identify potential workplace discrimination patterns using AI and statistical methods, generating insights and data visualizations for various demographic groups.

## Input Details
The workflow is manually triggered and begins by setting a company name (e.g., "Twilio") for analysis.

## Process Summary
The workflow starts by scraping Glassdoor for company review data using ScrapingBee, extracting overall review summaries and demographic-specific content. It then uses OpenAI to extract detailed ratings and review counts for various demographic groups. Subsequently, it calculates statistical measures like variance, standard deviation, Z-scores, effect sizes, and P-scores to quantify potential biases. Finally, it leverages AI to generate a textual analysis of the bias data, including key takeaways and employee experience perceptions, and produces a bar chart and a scatterplot visualization of the findings using QuickChart.

## Output Details
The workflow produces an AI-generated text analysis of workplace bias, a bar chart visualizing demographic effect sizes, and a scatterplot showing Z-scores and effect sizes for different demographic groups.
