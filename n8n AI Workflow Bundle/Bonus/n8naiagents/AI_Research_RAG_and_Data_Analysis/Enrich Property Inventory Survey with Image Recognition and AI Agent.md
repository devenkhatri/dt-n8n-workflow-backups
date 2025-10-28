# Workflow Analysis for AI‑Powered Enrichment of Airtable Product Photos

## Description
This workflow scans an Airtable table for rows that contain a product photo but have not yet been processed, uses OpenAI's vision model to describe the object, runs an AI agent equipped with reverse‑image search and web‑scraping tools to gather missing attributes, parses the structured result, and writes the enriched data back into the Airtable record.

## Input Details
Manually triggered workflow that reads rows from Airtable where an image exists and AI_status is false.

## Process Summary
1) The manual trigger queries Airtable for applicable rows. 2) Each row’s image is sent to OpenAI’s vision model to generate an initial description. 3) An OpenAI agent, using the reverse‑image search tool (SerpAPI) and the webpage scraper tool (Firecrawl), gathers additional product details and returns a structured JSON payload. 4) The Structured Output Parser extracts fields like title, model, material, color, and condition. 5) The workflow updates the original Airtable record with the enriched attributes and marks it as processed.

## Output Details
Enriched product information is written back to the same Airtable record, updating fields such as Title, Description, Model, Material, Color, Condition, and setting AI_status to true.
