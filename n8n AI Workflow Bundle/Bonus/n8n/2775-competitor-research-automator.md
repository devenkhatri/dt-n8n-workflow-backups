# Workflow Analysis for Competitor Research Automator

## Description
This workflow automates the process of competitor research by gathering information from Google Search, analyzing website content with AI, and extracting key data points.

## Input Details
The workflow is manually triggered and receives a list of competitor URLs as input.

## Process Summary
The workflow iterates through each provided competitor URL. For each URL, it performs a Google search to find the competitor's website, retrieves the content of the website, applies an AI model to analyze the content, and extracts relevant information such as the business model and target audience. Finally, it uses another AI model to summarize the extracted information for each competitor.

## Output Details
The workflow outputs a summary of competitor research, including business model and target audience, to a Google Sheet.
