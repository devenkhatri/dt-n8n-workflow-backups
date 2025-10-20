# Workflow Analysis for Glassdoor Discrimination Analysis

## Description
This workflow analyzes Glassdoor reviews for potential discrimination using AI, categorizes them, and stores the results in Google Sheets.

## Input Details
The workflow is triggered by an HTTP request, receiving data that includes Glassdoor review URLs, API keys, and Google Sheet credentials.

## Process Summary
The workflow starts by extracting review data from the provided Glassdoor URLs. Then, it uses an AI model to evaluate each review for potential discrimination and categorize it. After processing, the analysis results are formatted and appended to a specified Google Sheet, with an additional step to ensure proper data handling and error logging.

## Output Details
The workflow outputs the discrimination analysis results, including categories and AI assessment, to a Google Sheet.
