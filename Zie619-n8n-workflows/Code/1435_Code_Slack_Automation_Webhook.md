# Workflow Analysis for piepdrive-test

## Description
This workflow automatically enriches newly created Pipedrive organization records by scraping their website content, using AI to generate a detailed company summary, saving it as a note in Pipedrive, and notifying a Slack channel with the enriched data.

## Input Details
The workflow is triggered when a new organization is created in Pipedrive and receives the organization's data, including a custom website field.

## Process Summary
When a new organization is added in Pipedrive, the workflow scrapes the organization’s website using ScrapingBee. The scraped HTML content is sent to OpenAI’s GPT-4o model, which generates a structured HTML summary including company description, target market, unique selling points, and potential competitors. This AI-generated summary is then added as a note to the Pipedrive organization. The HTML note is converted to Markdown and then formatted for Slack before being sent to a designated Slack channel.

## Output Details
The workflow creates a detailed AI-generated note in Pipedrive and sends a formatted version of that note to a Slack channel for team visibility.

## Tags
Pipedrive, OpenAI, GPT-4o, web scraping, Slack notification, CRM enrichment, automation, n8n, production-ready
