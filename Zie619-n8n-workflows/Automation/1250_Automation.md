# Workflow Analysis for Airtable Assistant with OpenAI Integration

## Description
This workflow acts as an intelligent assistant that processes user queries about Airtable data using OpenAI. It interprets natural language requests, identifies the correct Airtable base and tables, retrieves or aggregates data as needed, and can even generate visualizations like maps based on the request.

## Input Details
The workflow is triggered manually or via chat message input containing a natural language query about Airtable data.

## Process Summary
The workflow starts by receiving a user query, then uses OpenAI with a custom system prompt to understand the request and determine required actions. It may fetch Airtable base and table schemas, search records, or execute custom code for aggregations or image generation. The workflow includes logic to handle missing filters, validate base/table IDs, and ensure accurate responses. Results are formatted and returned to the user, potentially including links to generated files or visualizations.

## Output Details
The workflow produces a structured response to the user’s query, which may include data from Airtable, aggregated results, or links to generated visual assets like map images.

## Tags
Airtable, OpenAI, chat assistant, data query, automation, aggregation, visualization, n8n
