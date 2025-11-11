# Workflow Analysis for Automate Competitor Research with Exa.ai, Notion and AI Agents

## Description
This workflow automatically identifies competitors of a given company using Exa.ai, then uses AI-powered agents to gather detailed information about each competitor including company overview, product offerings, and customer reviews. The collected data is structured and saved into a Notion database for easy analysis and reporting.

## Input Details
The workflow is manually triggered and starts with a user-defined source company URL (e.g., https://notion.so).

## Process Summary
First, the workflow uses Exa.ai's findSimilar API to discover up to 10 competitor companies based on the provided source company URL. It then processes each competitor one by one through three specialized AI agents. The Company Overview Agent gathers funding, leadership, and organizational details by scraping Crunchbase, WellFound, and LinkedIn. The Company Product Offering Agent researches product features, pricing, and plans by searching and scraping the competitor's website. The Company Product Reviews Agent finds and analyzes customer reviews from sites like Trustpilot and Product Hunt. Finally, all collected data is merged and formatted into a structured report.

## Output Details
The workflow creates a comprehensive competitor analysis report and inserts it as a new entry in a specified Notion database, including rich text content and structured properties.

## Tags
competitor research, market analysis, AI agent, Exa.ai, Notion, web scraping, company data, product research, customer reviews, automation
