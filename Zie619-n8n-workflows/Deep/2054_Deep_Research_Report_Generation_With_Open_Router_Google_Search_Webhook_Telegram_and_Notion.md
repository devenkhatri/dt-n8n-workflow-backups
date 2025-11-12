# Workflow Analysis for Deep Research Report Generation Using Open Router, Google Search, Webhook/Telegram and Notion

## Description
This workflow automates the end-to-end process of generating in-depth research reports based on user input. It starts by collecting a research topic via Telegram or a webhook, clarifies the scope through follow-up questions, generates targeted search queries, fetches and analyzes relevant web content, and finally compiles a well-structured, cited report saved to Notion.

## Input Details
The workflow is triggered by either a Telegram message or an HTTP webhook request containing a user's research topic or response.

## Process Summary
First, the Strategy Agent interacts with the user to define and confirm a research plan. Once confirmed, the Search Query Agent generates up to three precise search queries. For each query, the workflow calls an external search API (like Tavily), identifies the most relevant URL using an AI model, and extracts detailed content from it. The AI Agent then synthesizes all extracted content into a comprehensive markdown report with proper citations. This report is converted into Notion-compatible blocks and stored in a Notion database, with status updates sent via HTTP request.

## Output Details
The workflow produces a detailed research report in markdown format, saves it as formatted content in a Notion database page, updates the page status to 'Done', and sends a notification with the report title and URL via an HTTP callback.

## Tags
research automation, AI report generation, Notion integration, Telegram bot, webhook trigger, web scraping, content synthesis, OpenRouter, Tavily API, markdown to Notion
