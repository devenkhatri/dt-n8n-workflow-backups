# Workflow Analysis for AI-Powered Product Attribute Extraction from Survey Photos

## Description
This workflow automatically analyzes product photos from an Airtable survey, uses AI vision to identify product attributes, enhances the analysis by performing reverse image searches and web scraping, and then updates the original Airtable records with enriched product information like title, description, model, material, color, and condition.

## Input Details
The workflow is triggered manually and fetches rows from an Airtable base that contain images and have not yet been processed by AI (AI_status = FALSE).

## Process Summary
First, the workflow retrieves applicable rows from Airtable with unprocessed product images. It then uses OpenAI's vision model to analyze each image and extract initial product attributes. An AI agent subsequently refines this data by optionally performing a reverse image search via SERP API or scraping relevant webpages using Firecrawl. Based on the agent's structured output, the workflow updates the corresponding Airtable row with the enriched product details and marks it as processed.

## Output Details
The workflow updates the original Airtable rows with extracted and verified product attributes (title, description, model, material, color, condition) and sets the AI_status flag to true.

## Tags
AI Vision, Airtable, OpenAI, Reverse Image Search, Web Scraping, Product Recognition, Workflow Automation, LangChain Agent
