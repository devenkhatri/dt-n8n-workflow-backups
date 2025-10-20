# Workflow Analysis for AI SEO Keyword Automation

## Description
This workflow leverages AI to expand a given set of SEO keywords and then gathers detailed search metrics for each new keyword, finally exporting the data to a Google Sheet.

## Input Details
The workflow is triggered on a scheduled interval (e.g., monthly) and starts with a predefined keyword or topic along with target audience and search intent.

## Process Summary
First, the workflow uses OpenAI to generate 10-20 long-tail keywords based on the initial input, target audience, and search intent. Then, it splits these generated keywords into individual items. For each keyword, it makes an HTTP request to a RapidAPI endpoint to retrieve search volume, CPC, and competition data. After fetching the data, it structures the relevant keyword information. Finally, it appends this structured data as a new row in a specified Google Sheet.

## Output Details
The workflow outputs an updated Google Sheet with new keywords and their corresponding search volume, CPC, competition, and other search metrics.
