# Workflow Analysis for Google analytics template

## Description
This workflow automatically pulls Google Analytics data for the current and previous weeks across three categories—page engagement, Google Search Console results, and country-based views—sends the comparisons to an AI model for analysis, and saves the AI-generated SEO insights to a Baserow database.

## Input Details
The workflow is triggered either on a weekly schedule or manually, and it pulls data directly from Google Analytics using a configured property ID.

## Process Summary
The workflow first fetches page engagement, search console, and country view metrics for both the current and prior weeks from Google Analytics. It then transforms each dataset into a simplified, URL-encoded JSON format. These formatted datasets are sent to an AI service (via HTTP POST) with a prompt asking for a markdown comparison table and SEO improvement suggestions. Finally, the AI responses for all three data types are saved as a new record in a Baserow table.

## Output Details
The workflow saves AI-generated SEO analysis (including markdown tables and suggestions) for page views, search performance, and country views into a Baserow database table.

## Tags
Google Analytics, SEO, AI analysis, Baserow, automation, scheduled workflow, data comparison, n8n
