# Workflow Analysis for Trustpilot Customer Insights Dashboard Builder

## Description
This workflow automates the process of collecting Trustpilot reviews, analyzing their sentiment and themes using AI, and then compiling these insights into a Google Sheet for reporting and a detailed Google Doc for individual review analysis.

## Input Details
This workflow is triggered manually.

## Process Summary
The workflow starts by retrieving reviews from Trustpilot for a specified business. It then uses an AI model to perform sentiment analysis and extract key themes from each review. Next, it structures this analyzed data into a format suitable for a Google Sheet, creating a new sheet if one doesn't exist and appending the data. Additionally, it generates a comprehensive summary for each review, including sentiment, key takeaways, and suggested improvements, and compiles these into a neatly formatted Google Document.

## Output Details
The workflow outputs a Google Sheet containing structured review data and a Google Document with detailed AI-generated insights for each Trustpilot review.
