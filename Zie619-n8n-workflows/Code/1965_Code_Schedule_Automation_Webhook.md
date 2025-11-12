# Workflow Analysis for SERPBear analytics template

## Description
This workflow automatically fetches SEO keyword ranking data from SERPBear for a specific website, analyzes the trends using an AI model, and saves the insights into a Baserow database for tracking and reporting.

## Input Details
The workflow is triggered either manually or on a weekly schedule and receives no external input data—it uses predefined configuration like the target domain and API credentials.

## Process Summary
The workflow starts by fetching SEO keyword ranking data from SERPBear via an HTTP request. It then processes this data in a code node to calculate current positions, 7-day averages, and trend directions for each keyword. This summarized data is formatted into a prompt and sent to an AI service (via HTTP POST) for expert-level analysis and recommendations. The AI’s response is parsed and stored in a Baserow table along with the current date and website name. The entire process includes robust error handling and is designed for weekly automated execution.

## Output Details
The workflow saves the AI-generated SEO analysis as a new record in a Baserow table, including the date, analysis content, and associated website name.

## Tags
SEO, SERPBear, AI analysis, Baserow, automation, weekly report, n8n, production-ready
