# Workflow Analysis for Dynamic Webpage Generation with OpenAI

## Description
This workflow dynamically creates a webpage based on user input by leveraging OpenAI's structured output capabilities to generate HTML content, which is then rendered and returned to the user.

## Input Details
The workflow is triggered by an HTTP request via a webhook, receiving user input as a query parameter named "query".

## Process Summary
First, the workflow receives a user query via an HTTP webhook. It then sends this query to OpenAI with a specific prompt requesting HTML code for a webpage, enforcing JSON output for structured content. Next, it parses the JSON response from OpenAI to extract the generated HTML. Finally, it constructs an HTML response with the generated content and adds a CSS style for basic page appearance.

## Output Details
The workflow returns a dynamically generated HTML webpage as an HTTP response to the user.
