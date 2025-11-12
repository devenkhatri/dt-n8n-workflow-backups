# Workflow Analysis for LinkedIn Web Scraping with Bright Data MCP Server & Google Gemini

## Description
This workflow scrapes LinkedIn person and company profiles using Bright Data's MCP tools, processes the scraped data with Google Gemini to generate a narrative story about the company, and saves or sends the results via webhook and local file storage.

## Input Details
The workflow is triggered manually and uses URLs from environment variables to scrape LinkedIn profiles for a person and a company.

## Process Summary
The workflow starts with a manual trigger, then sets LinkedIn profile URLs from environment variables. It uses Bright Data's MCP client to scrape both person and company LinkedIn profiles. The scraped person data is written to a local JSON file and sent via webhook. The company data is parsed, merged with additional fields, and passed to Google Gemini through a no-op node configured as a prompt to generate a company story. The final company data, including the generated story, is aggregated, saved to a local file, and sent via another webhook.

## Output Details
The workflow outputs scraped and processed LinkedIn person and company data as JSON files on disk and sends them to external endpoints via HTTP webhooks.

## Tags
LinkedIn, web scraping, Bright Data, Google Gemini, MCP, automation, n8n, production-ready, data extraction, AI generation
