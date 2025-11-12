# Workflow Analysis for Google Analytics SEO Insights Workflow

## Description
This workflow automatically retrieves Google Analytics data for the current and previous week, compares page engagement, search console performance, and country-level traffic, then sends the comparison to an AI service for SEO insights and saves the results to a Baserow database.

## Input Details
The workflow is triggered either on a weekly schedule or manually, and it pulls data from a configured Google Analytics GA4 property using a predefined property ID.

## Process Summary
First, the workflow fetches page engagement metrics (like views, users, and events) for both this week and the prior week. Separately, it retrieves Google Search Console data (such as clicks, impressions, and CTR) and country-level user statistics for the same periods. All data is parsed and formatted into simplified JSON strings. These are then sent via HTTP POST requests to an AI model (Llama 3.1) with instructions to compare the two weeks and generate SEO recommendations in markdown. Finally, the AI’s responses for all three data categories are saved as a new record in a Baserow table.

## Output Details
The workflow saves structured AI-generated SEO insights—including markdown tables and actionable suggestions for page engagement, search performance, and country traffic—into a Baserow database.

## Tags
google analytics, SEO, AI analysis, automation, Baserow, weekly report, n8n, production-ready, data comparison, Llama AI
