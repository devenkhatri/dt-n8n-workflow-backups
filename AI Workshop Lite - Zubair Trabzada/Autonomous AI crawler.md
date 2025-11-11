# Workflow Analysis for Autonomous AI Web Crawler for Social Media Links

## Description
This workflow automatically crawls company websites to find and extract social media profile links, then stores the results in a database.

## Input Details
The workflow is triggered manually and receives company data (name and website URL) from a Supabase database table called 'companies_input'.

## Process Summary
The workflow retrieves company names and websites from a Supabase database, then uses an AI agent with OpenAI's GPT-4o to crawl each website. The AI agent has two custom tools: one to extract all text from a webpage and another to retrieve all URLs/links from a webpage. The agent analyzes this data to identify social media profile links, which are parsed into a standardized JSON format. Finally, the original company data is merged with the extracted social media links and saved to a 'companies_output' table in Supabase.

## Output Details
The workflow produces structured social media profile links for each company and stores them in a Supabase database table called 'companies_output'.

## Tags
web crawler, social media extraction, AI agent, OpenAI, GPT-4, website scraping, Supabase, URL extraction, data enrichment, automation
