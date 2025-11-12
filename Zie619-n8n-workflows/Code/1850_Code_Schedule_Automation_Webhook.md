# Workflow Analysis for Umami analytics template

## Description
This workflow automatically fetches website analytics data from Umami, processes it, sends it to an AI model for SEO insights and comparison between weeks, and saves the resulting analysis into a Baserow database.

## Input Details
The workflow is triggered either manually or on a weekly schedule (every Thursday) and fetches analytics data from the Umami API using configured environment variables and credentials.

## Process Summary
First, the workflow retrieves high-level website metrics (pageviews, visitors, etc.) from Umami and formats them using a code node. This data is sent to an AI service (via OpenRouter) to generate a markdown summary. Separately, it fetches page-specific stats for the current and previous weeks, encodes them, and sends both datasets to the AI for a comparative analysis with improvement suggestions. Finally, both AI-generated summaries are saved into a Baserow table along with the current date and blog name.

## Output Details
The workflow saves two AI-generated analyses (overall summary and week-over-week comparison) into a Baserow database table with fields for date, summary, top pages, and blog name.

## Tags
Umami, analytics, AI, SEO, Baserow, automation, weekly report, n8n, production-ready, OpenRouter
