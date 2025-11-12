# Workflow Analysis for Google analytics template

## Description
This workflow automatically retrieves Google Analytics data for the current and previous week across three key areas—page engagement, Google Search Console performance, and country-wise user views—compares the metrics using an AI model, and stores the AI-generated SEO insights and markdown reports in a Baserow database.

## Input Details
The workflow is triggered either on a weekly schedule or manually, and it pulls data from a configured Google Analytics property (via OAuth credentials) using a predefined property ID.

## Process Summary
The workflow first fetches page engagement stats, Google Search Console metrics, and country-level user data for both the current week and the prior week from Google Analytics. It then processes and simplifies this data using code nodes, encoding it into URL-safe JSON strings. These data strings are sent to an external AI service (via HTTP POST) with a prompt asking for a comparative markdown table and SEO suggestions. Finally, the AI responses for all three data categories are saved into a Baserow database table with a timestamp.

## Output Details
The workflow produces AI-generated SEO analysis (in markdown format) for page engagement, search performance, and geographic traffic trends, and saves these results along with a timestamp to a specified Baserow database table.

## Tags
google analytics, SEO analysis, AI integration, Baserow, automation, data comparison, weekly report, n8n
