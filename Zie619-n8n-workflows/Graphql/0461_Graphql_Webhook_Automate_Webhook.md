# Workflow Analysis for Production Workflow

## Description
This workflow retrieves country information (name, phone code, and emoji) based on a provided country code and returns a formatted message with the details.

## Input Details
The workflow is triggered by a webhook that receives a country code as a query parameter.

## Process Summary
The workflow starts with a webhook that captures a country code from the query parameters. It then sends a GraphQL query to an external API endpoint to fetch country details like name, phone code, and emoji. The raw JSON response is parsed using a Function node to extract the relevant country data. Finally, a Set node formats this data into a human-readable sentence containing the country name, emoji, and phone code.

## Output Details
The workflow outputs a formatted message containing the country name, emoji, and phone code, which is returned as the webhook response.

## Tags
webhook, graphql, country-data, formatting, production-ready, error-handling
