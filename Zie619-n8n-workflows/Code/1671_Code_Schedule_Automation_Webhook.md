# Workflow Analysis for Umami analytics template

## Description
This workflow automatically fetches website analytics data from Umami, analyzes it using an AI model, compares weekly performance, and saves a summarized report to a Baserow database for tracking and insights.

## Input Details
The workflow is triggered either manually or automatically every Thursday via a schedule trigger, and it pulls analytics data from the Umami API using configured environment variables and authentication headers.

## Process Summary
First, the workflow retrieves high-level website metrics (pageviews, visitors, etc.) from Umami. It then formats this data and sends it to an AI model (via OpenRouter) to generate a summary table. Next, it fetches detailed page-specific stats for both the current and previous week, encodes the data, and sends it to the AI for a comparative analysis with improvement suggestions. Finally, both the summary and comparison results are saved into a Baserow table along with the current date and blog name.

## Output Details
The workflow saves structured analytics insights—including a summary, top pages analysis, date, and blog name—into a predefined Baserow database table.

## Tags
Umami, analytics, AI analysis, Baserow, automation, SEO, weekly report, n8n, production-ready, OpenRouter
