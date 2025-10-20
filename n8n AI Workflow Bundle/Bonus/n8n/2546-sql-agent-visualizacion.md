# Workflow Analysis for SQL Agent Visualization Workflow

## Description
This workflow serves as a proof of concept for interacting with a SQL database using a natural language interface, generating SQL queries, executing them, and visualizing the results.

## Input Details
Input is received via a webhook, triggered by an HTTP POST request containing a "question" field in its body.

## Process Summary
The workflow starts by extracting a natural language question from the incoming webhook. It then uses an AI model to convert this natural language question into a SQL query. This generated SQL query is then executed against a specified SQL database. Finally, the results of the SQL query are taken and processed to remove sensitive information before being returned as a response.

## Output Details
The workflow returns the processed results of the SQL query as an HTTP response.
