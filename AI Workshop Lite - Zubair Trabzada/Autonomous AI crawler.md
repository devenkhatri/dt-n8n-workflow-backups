# Workflow Analysis for Autonomous AI Web Crawler for Social Media Profile Links

## Description
This workflow uses an autonomous AI agent to crawl company websites, extract social media profile links, and store them in a structured format within a database.

## Input Details
The workflow is manually triggered and retrieves company names and websites from a Supabase table named "companies_input."

## Process Summary
The workflow starts by fetching company details (name and website) from a Supabase database. For each company, an AI agent is invoked to autonomously crawl its website. This agent utilizes specialized tools to retrieve text content and URLs from webpages. It processes the website, identifies social media links, and structures them into a predefined JSON format using an OpenAI chat model and a JSON parser. The extracted social media data is then merged with the original company information.

## Output Details
The workflow inserts the original company data, along with the newly extracted social media profile links, into a Supabase table named "companies_output."
