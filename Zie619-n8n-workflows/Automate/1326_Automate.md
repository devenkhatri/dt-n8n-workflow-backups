# Workflow Analysis for Competitor Analysis and Company Review Aggregator

## Description
This workflow automatically gathers and analyzes online reviews and product information for a specified company or its competitors, then stores the structured insights in a Notion database.

## Input Details
The workflow is triggered manually and receives no external input data other than the initiation signal.

## Process Summary
The workflow starts with a manual trigger and proceeds to collect company-related data by searching review sites, social media, and business directories like Crunchbase, LinkedIn, and WellFound. It uses AI agents to extract structured information such as number of reviews, sentiment percentages, top pros/cons, and geographic sources. Duplicate results are filtered out, and the final aggregated data is formatted according to a predefined schema. The cleaned and structured output is then inserted into a Notion database for further analysis or reporting.

## Output Details
The workflow outputs structured company review and product offering data and saves it as a new entry in a configured Notion database.

## Tags
competitor analysis,review aggregation,Notion integration,AI agent,web scraping,company research,structured output,manual trigger
