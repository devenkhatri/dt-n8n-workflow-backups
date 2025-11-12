# Workflow Analysis for SERPBear analytics template

## Description
This workflow automatically retrieves SEO keyword ranking data from SERPBear for a specific domain, analyzes trends using an AI model, and saves the AI-generated insights into a Baserow database for tracking and reporting.

## Input Details
The workflow is triggered either manually or on a weekly schedule, and it fetches SEO ranking data from the SERPBear API for the domain 'rumjahn.com'.

## Process Summary
The workflow starts by fetching raw keyword ranking data from SERPBear via an HTTP request. It then processes this data in a code node to calculate current position, 7-day average position, and trend (improving, declining, or stable) for each keyword. This processed data is formatted into a prompt and sent to an AI model (via OpenRouter) for expert SEO analysis. The AI's response, containing summarized insights and recommendations, is then stored in a Baserow table along with the current date and site name.

## Output Details
The workflow saves the AI-generated SEO analysis as a new record in a Baserow table with fields for date, analysis note, and blog name.

## Tags
SEO, SERPBear, AI analysis, Baserow, automation, weekly report, keyword tracking, n8n
