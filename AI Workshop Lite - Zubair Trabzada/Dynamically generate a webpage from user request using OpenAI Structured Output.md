# Workflow Analysis for Dynamically generate HTML page from user request using OpenAI Structured Output

## Description
This workflow creates a complete HTML web page based on a user's natural language request by leveraging OpenAI's structured output capabilities to ensure consistent and predictable results.

## Input Details
The workflow is triggered by a webhook that receives a user's text query via a URL parameter named 'query'.

## Process Summary
The workflow starts by receiving a user query through a webhook. It sends this query to OpenAI's GPT-4o model with a strict JSON schema defining UI components and Tailwind CSS attributes. The structured JSON response is then passed to another OpenAI call that converts it into raw HTML and a page title. This HTML is embedded into a full HTML document template that includes the Tailwind CSS CDN. Finally, the complete HTML page is returned as the webhook response.

## Output Details
The workflow outputs a fully rendered HTML page with Tailwind styling, which is sent directly back to the user's browser as the webhook response.

## Tags
OpenAI, HTML generation, structured output, GPT-4o, Tailwind CSS, webhook, AI design, dynamic content
